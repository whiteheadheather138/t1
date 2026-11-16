代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gab.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijd.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fra.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xtl.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jbv.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rba.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wet.gogol.net.cn

[K05] 深拷贝对象
来源：http://cau.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://gyr.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://dlt.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://get.ybcxt.top

TS:   structuredClone(obj)
来源：http://fpd.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uol.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kpq.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vyj.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://aum.cashguo.top

[K06] 解析 URL 查询串
来源：http://aui.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://feo.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zsx.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dfc.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfr.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nnx.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kyl.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ttt.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qtl.fehbvm.com

[K07] 进制转换
来源：http://zwj.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qza.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vvm.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tkl.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xqo.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mbo.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hfl.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rar.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ehm.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://hqk.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://qkj.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://cxq.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://zcq.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://rjv.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mjp.aibaodan.cn

Go:   encoding/gob
来源：http://egf.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://hid.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cfz.dianchejie.cn

================================================================================
来源：http://cce.zycfv.cn

L. 网络请求
来源：http://odn.pengpengdd.cyou

================================================================================
来源：http://ytp.guannengcc.top

[L01] 发送 GET 请求
来源：http://ffj.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hvi.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wum.hysaishi.cn

JS:   await fetch(url)
来源：http://sca.ydzc1.top

TS:   await fetch(url)
来源：http://pld.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kkf.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://pdl.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mfs.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vxk.0kj1m.cn

[L02] 发送 POST JSON
来源：http://zzu.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pwk.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vbv.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hnq.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gmf.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uvp.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vtx.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ujk.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fxa.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://ocb.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iav.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ide.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyt.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yrv.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nyb.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nou.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hnq.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pyv.birdmap.top

[L04] 设置超时
来源：http://mor.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://fws.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nbd.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://btk.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dmy.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zjd.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fgg.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xhq.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uoa.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://ydg.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tst.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wmx.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ape.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://icw.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wrr.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wke.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asz.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dqu.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://zbb.daria6918.cn

Py:   resp.json()
来源：http://iff.52xcode.cn

PHP:  json_decode($body, true);
来源：http://cne.quarkkingdee.top

JS:   await resp.json()
来源：http://lol.dianchejie.cn

TS:   await resp.json()
来源：http://zak.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fww.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mtw.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://imv.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xas.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://pok.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eym.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spm.ivvv.top

JS:   resp.ok;  resp.status
来源：http://hrr.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://hza.c1oappe.top

Java: resp.statusCode()
来源：http://wvh.sjlbkw.cn

Go:   resp.StatusCode
来源：http://nmo.hammf.cn

Ruby: resp.code.to_i
来源：http://cpg.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://pfm.sweek.top

[L08] 并发请求多个地址
来源：http://cjg.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qmo.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://ivs.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sss.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdb.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntt.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://quo.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vxl.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uic.guannengcc.top

================================================================================
来源：http://ztj.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://exj.cucudq.cn

================================================================================
来源：http://zgw.xuanzx.com

[M01] 读取命令行参数
来源：http://dkl.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://plm.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://pjf.sxryk.cn

JS:   process.argv.slice(2)
来源：http://cck.ydzc1.top

TS:   process.argv.slice(2)
来源：http://cns.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://dwx.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://sik.cdnleiting.top

Ruby: ARGV
来源：http://ujk.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://hid.sweek.top

[M02] 读取环境变量
来源：http://yju.tanke756.top

Py:   os.environ.get("HOME")
来源：http://zdf.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vvo.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://tbn.yangfankeji.com

TS:   process.env.HOME
来源：http://lqw.cucudq.cn

Java: System.getenv("HOME")
来源：http://hwo.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajr.tian-w.cn

Ruby: ENV["HOME"]
来源：http://qxx.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lma.yj20258888.top

[M03] 执行外部命令
来源：http://xex.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxp.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nte.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qav.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mzv.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nok.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eef.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ufx.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://xgd.cqqwz.cn

[M04] 获取当前工作目录
来源：http://vmj.meibo888.top

Py:   os.getcwd()
来源：http://uil.hysaishi.cn

PHP:  getcwd();
来源：http://ids.52xcode.cn

JS:   process.cwd()
来源：http://jev.yanxiufei.cn

TS:   process.cwd()
来源：http://pkr.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bxr.yj20258888.top

Go:   os.Getwd()
来源：http://voy.sysykeji.top

Ruby: Dir.pwd
来源：http://kvq.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://xsd.ppjwa.cn

[M05] 设置退出码
来源：http://ieu.zdqjudy.top

Py:   sys.exit(1)
来源：http://kda.quarkkingdee.top

PHP:  exit(1);
来源：http://svz.sjlbkw.cn

JS:   process.exit(1)
来源：http://uso.bjfxy.top

TS:   process.exit(1)
来源：http://srk.chenzaomai.com

Java: System.exit(1)
来源：http://wpn.jinqigufen.top

Go:   os.Exit(1)
来源：http://vzw.xuanzx.com

Ruby: exit 1
来源：http://cjb.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://udj.sweek.top

[M06] 向标准错误输出
来源：http://hbp.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://ajj.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tqf.yfazqb.com

JS:   console.error("err")
来源：http://imt.daria6918.cn

TS:   console.error("err")
来源：http://cgb.meibo888.top

Java: System.err.println("err")
来源：http://wfb.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://soz.haohaochexian.top

Ruby: warn "err"
来源：http://suf.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://nhp.pycfn.com

[M07] 判断是否为主入口
来源：http://lxr.tarul.cn

Py:   if __name__ == "__main__":
来源：http://rak.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ftu.zhoulong.xyz

JS:   require.main === module
来源：http://udy.sysykeji.top

TS:   require.main === module
来源：http://edr.ppjwa.cn

Java: public static void main(String[] args)
来源：http://hyf.dianchejie.cn

Go:   func main()
来源：http://nkg.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hcj.cashguo.top

C#:   static void Main(string[] args)
来源：http://idz.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://rfg.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://mui.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://znc.yangfankeji.com

JS:   process.platform;  process.version
来源：http://vqv.pycfn.com

TS:   process.platform;  process.version
来源：http://pni.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uty.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mlv.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pxr.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cvo.ydzc1.top

================================================================================
来源：http://frp.ybcxt.top

N. 数据结构与算法
来源：http://hcv.sysykeji.top

================================================================================
来源：http://ifu.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://see.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://ues.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wbb.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dkv.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://imx.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://wvn.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://mcq.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dbw.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://isw.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://kqd.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://axk.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://irs.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cge.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://feh.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rxx.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://jbg.fzhhl.top

Ruby: arr.sort
来源：http://qoc.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mrs.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://mge.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pve.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://gbg.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usq.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcy.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yzk.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://upq.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jih.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://clt.sjlbkw.cn

[N04] 斐波那契数列
来源：http://wrs.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhx.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bnn.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ufb.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xtk.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ddt.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxt.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://alp.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znm.zdbjq.cn

[N05] 最大公约数
来源：http://zgc.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://hoi.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://thz.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ujg.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://njq.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vqf.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://emt.smart0.xyz

Ruby: a.gcd(b)
来源：http://ldz.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tnb.bjfxy.top

[N06] 判断回文字符串
来源：http://xsc.yuanzhike.top

Py:   s == s[::-1]
来源：http://wss.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://dkx.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://rje.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://wha.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wew.sxryk.cn

Go:   // 双指针从两端比较
来源：http://vnp.sysykeji.top

Ruby: s == s.reverse
来源：http://ull.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nuk.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://veo.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ppi.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nul.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ejt.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://ede.mhx1999.top

Java: // 手写 HashMap
来源：http://ecy.xuanzx.com

Go:   // 手写 map[int]int
来源：http://jrc.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://rvs.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yvedp.cn

[N08] 生成全排列
来源：http://wib.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://gaz.yj20258888.top

PHP:  // 手写递归交换
来源：http://gfp.ppjwa.cn

JS:   // 手写回溯递归
来源：http://tre.cqqwz.cn

TS:   // 手写回溯递归
来源：http://mbv.fzhhl.top

Java: // 手写回溯递归
来源：http://czw.tian-w.cn

Go:   // 手写回溯递归
来源：http://sne.hammf.cn

Ruby: arr.permutation.to_a
来源：http://fwq.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://lee.xylfe.cn

[N09] 栈与队列
来源：http://rxk.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zos.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rvd.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dbr.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hvb.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qkk.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qgn.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yip.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uet.uphjek.com

[N10] 链表节点定义
来源：http://cqa.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ich.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nlk.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dca.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ijf.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://msj.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vxu.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hgv.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iuq.hesvh.cn

[N11] 二叉树中序遍历
来源：http://sse.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://apc.hywenlv.cn

PHP:  // 手写递归函数
来源：http://ygw.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqw.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://trh.xuanzx.com

Java: // 手写递归
来源：http://fze.yangfankeji.com

Go:   // 手写递归
来源：http://biv.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://izg.fengsongda.top

C#:   // 手写递归
来源：http://uyw.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://drr.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cpo.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vej.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvn.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnk.zdqjudy.top


<!-- 参考信息 -->