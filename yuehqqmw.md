代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://itz.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://txq.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ffh.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myh.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jbe.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://znu.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tju.meibo888.top

[K05] 深拷贝对象
来源：http://dho.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://gsn.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://urt.nanxinkj.top

JS:   structuredClone(obj)
来源：http://qgc.guowangkeji.top

TS:   structuredClone(obj)
来源：http://xng.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lgw.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njx.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nwj.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fie.hnqzz.top

[K06] 解析 URL 查询串
来源：http://kon.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jpj.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zub.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gcr.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vgw.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://czz.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ijb.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gtx.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dqy.chenzaomai.com

[K07] 进制转换
来源：http://ofu.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dvz.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://inb.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qax.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ykg.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ktk.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ufy.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iql.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gdp.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://mbe.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://rjp.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gtm.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://pok.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://hnc.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zcc.c1oappe.top

Go:   encoding/gob
来源：http://yfs.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://wjc.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wqa.xingfuxueyuan.xyz

================================================================================
来源：http://dwc.gaohongyu789.top

L. 网络请求
来源：http://mog.shanyushiyangkeji.top

================================================================================
来源：http://ugx.fehbvm.com

[L01] 发送 GET 请求
来源：http://lji.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://udj.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkt.quarkkingdee.top

JS:   await fetch(url)
来源：http://hkr.hongshengwenyu.top

TS:   await fetch(url)
来源：http://uqk.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cjn.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://tyz.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wih.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vpq.cheryme.top

[L02] 发送 POST JSON
来源：http://kok.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://znw.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vru.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifz.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trh.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qdr.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sld.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ozi.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://owl.pycfn.com

[L03] 设置自定义请求头
来源：http://vpd.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wqb.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qtk.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcs.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ouz.birdmap.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pyc.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ljc.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dld.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dxs.tanke756.top

[L04] 设置超时
来源：http://ocp.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://ypb.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lvf.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yag.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwi.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qph.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dux.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mnh.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ceg.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://hlt.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://odx.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rrf.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oju.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vvk.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mui.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cxp.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://agq.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://clf.uphjek.com

[L06] 解析响应为 JSON
来源：http://fzh.ydzc1.top

Py:   resp.json()
来源：http://nqn.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://ble.redwolf501.top

JS:   await resp.json()
来源：http://jaj.ivvv.top

TS:   await resp.json()
来源：http://acv.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gjb.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qzm.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://mvp.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gzl.ppjwa.cn

[L07] 处理 HTTP 状态码
来源：http://ueo.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hdg.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wtt.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://qnl.uphjek.com

TS:   resp.ok;  resp.status
来源：http://qcu.yuxming.cn

Java: resp.statusCode()
来源：http://kxw.svipenyu.cn

Go:   resp.StatusCode
来源：http://egh.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://lmx.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://igx.hesvh.cn

[L08] 并发请求多个地址
来源：http://udi.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uto.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://klp.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rsm.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dus.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rjx.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hyl.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://czd.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dco.vehdjk.com

================================================================================
来源：http://ank.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://nnd.zhoulong.xyz

================================================================================
来源：http://wle.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://aef.yfazqb.com

Py:   sys.argv[1:]
来源：http://iqv.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://gzn.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://fwx.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://phr.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://cay.jinqigufen.top

Go:   os.Args[1:]
来源：http://rje.haohaochexian.top

Ruby: ARGV
来源：http://ydf.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://nqv.sysykeji.top

[M02] 读取环境变量
来源：http://wjk.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://dcd.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dhw.ydjk.org.cn

JS:   process.env.HOME
来源：http://upy.yfazqb.com

TS:   process.env.HOME
来源：http://ogk.zdbjq.cn

Java: System.getenv("HOME")
来源：http://fag.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pnf.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://wpf.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://knk.aibaodan.cn

[M03] 执行外部命令
来源：http://svf.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lrr.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ehq.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://isa.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gzc.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oxv.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kho.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://xgh.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://fqs.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://qzj.pengpengdd.cyou

Py:   os.getcwd()
来源：http://sol.ydzc1.top

PHP:  getcwd();
来源：http://bha.fktsv.cn

JS:   process.cwd()
来源：http://gun.ybcxt.top

TS:   process.cwd()
来源：http://jaz.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://blm.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://wee.zhoulong.xyz

Ruby: Dir.pwd
来源：http://lgc.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mnp.yangfankeji.com

[M05] 设置退出码
来源：http://uuu.9152youxi.cn

Py:   sys.exit(1)
来源：http://ziq.vqdsnc.cn

PHP:  exit(1);
来源：http://xuz.tianlin.xyz

JS:   process.exit(1)
来源：http://vzc.ctjpmb.com

TS:   process.exit(1)
来源：http://viu.tarul.cn

Java: System.exit(1)
来源：http://mlg.xziqi.cn

Go:   os.Exit(1)
来源：http://crj.tianlin.xyz

Ruby: exit 1
来源：http://oxm.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jcq.fktsv.cn

[M06] 向标准错误输出
来源：http://uak.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://gmy.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jja.hysaishi.cn

JS:   console.error("err")
来源：http://yzr.bjfxy.top

TS:   console.error("err")
来源：http://ivb.bjfxy.top

Java: System.err.println("err")
来源：http://meo.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://idf.0kj1m.cn

Ruby: warn "err"
来源：http://ctr.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://xzh.yonumen.top

[M07] 判断是否为主入口
来源：http://txw.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://bne.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wtm.aibaodan.cn

JS:   require.main === module
来源：http://ojn.hysaishi.cn

TS:   require.main === module
来源：http://zeg.tian-w.cn

Java: public static void main(String[] args)
来源：http://sou.sjlbkw.cn

Go:   func main()
来源：http://ihj.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nam.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://wyw.316326.xyz

[M08] 获取系统与运行时信息
来源：http://nxs.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://bpb.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://dmx.hesvh.cn

JS:   process.platform;  process.version
来源：http://cxt.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://htx.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zqv.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nhh.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vre.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tix.ivvv.top

================================================================================
来源：http://xbj.daria6918.cn

N. 数据结构与算法
来源：http://ckc.zycfv.cn

================================================================================
来源：http://nak.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://xft.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://qdn.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baj.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlp.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://evh.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://uuu.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://hwm.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wjj.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nzr.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://bob.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://iro.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uqg.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ouz.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ljk.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hvh.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://woh.jinqigufen.top

Ruby: arr.sort
来源：http://ktc.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sol.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://pwu.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cbl.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://wum.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtx.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wiu.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lyh.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://azs.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mob.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://luo.snrcjt.cn

[N04] 斐波那契数列
来源：http://bwk.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://muh.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sjq.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcu.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvc.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nrv.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dgj.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ddy.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pgs.xziqi.cn

[N05] 最大公约数
来源：http://pus.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://uuz.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://irx.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snr.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vmu.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://osr.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sbo.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://egb.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwg.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://lgo.kuanghao11.cn

Py:   s == s[::-1]
来源：http://lfx.tanke756.top

PHP:  $s === strrev($s);
来源：http://htp.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://nxk.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://pux.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xgg.yonumen.top

Go:   // 双指针从两端比较
来源：http://fml.yj20258.top

Ruby: s == s.reverse
来源：http://mqd.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ysg.yj202588.top

[N07] 两数之和（返回下标）
来源：http://nnm.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cqr.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tsl.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://oem.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://lsd.sxryk.cn

Java: // 手写 HashMap
来源：http://fwp.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://sde.yuxming.cn

Ruby: // 手写 Hash
来源：http://kqa.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://pxe.yangfankeji.com

[N08] 生成全排列
来源：http://uvu.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://gsi.zdqjudy.top

PHP:  // 手写递归交换
来源：http://qvi.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://btl.snrcjt.cn

TS:   // 手写回溯递归
来源：http://czc.zdqjudy.top

Java: // 手写回溯递归
来源：http://tfb.jyoumei.cn

Go:   // 手写回溯递归
来源：http://jdl.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://gna.bbcook.cn

C#:   // 手写回溯递归
来源：http://iha.gogol.net.cn

[N09] 栈与队列
来源：http://tpe.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://txv.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wzt.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kcj.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayd.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vay.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sum.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ysv.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lxt.birdmap.top

[N10] 链表节点定义
来源：http://cmi.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xwp.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://otx.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hsy.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bul.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://wkn.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qvk.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eau.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nyc.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://oiw.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zjg.meibo888.top

PHP:  // 手写递归函数
来源：http://ezp.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjy.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dwy.hammf.cn

Java: // 手写递归
来源：http://tln.zhengqikj.top

Go:   // 手写递归
来源：http://sdd.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lsb.gotoacloud.top

C#:   // 手写递归
来源：http://muf.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qhv.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jwa.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ycg.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uab.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://euc.aibaodan.cn


<!-- 参考信息 -->