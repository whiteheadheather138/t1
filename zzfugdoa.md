代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://ovm.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bnn.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://upv.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qnx.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gwh.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hmt.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfo.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbu.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://guh.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lco.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lgg.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://unq.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://ptd.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://chg.tarul.cn

JS:   structuredClone(obj)
来源：http://hya.zycfv.cn

TS:   structuredClone(obj)
来源：http://sdm.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dfq.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rsd.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mql.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kdn.yfazqb.com

[K06] 解析 URL 查询串
来源：http://igx.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewp.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yrl.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qln.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fve.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://igm.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xsr.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://khs.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bpz.aibaodan.cn

[K07] 进制转换
来源：http://end.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://web.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rnj.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ypy.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nbw.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dhs.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcl.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://clk.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hyb.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://mxw.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://nvc.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wgf.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gfq.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://cta.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fzt.snrcjt.cn

Go:   encoding/gob
来源：http://yuv.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://pqq.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fat.fehbvm.com

================================================================================
来源：http://djp.feifeiyinyue.top

L. 网络请求
来源：http://iee.hcnkem.com

================================================================================
来源：http://oiv.hesvh.cn

[L01] 发送 GET 请求
来源：http://wnq.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ami.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://svs.zhijiandao.cn

JS:   await fetch(url)
来源：http://mid.feifeiyinyue.top

TS:   await fetch(url)
来源：http://mad.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://osg.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://pgt.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mla.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sik.nanxinkj.top

[L02] 发送 POST JSON
来源：http://jdk.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://ykj.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://smj.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvy.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://arb.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uuu.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aag.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xnp.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kpu.316326.xyz

[L03] 设置自定义请求头
来源：http://zav.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kkj.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fzp.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xhe.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ywu.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mox.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pte.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://etn.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eth.ydzc1.top

[L04] 设置超时
来源：http://mtv.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://fdj.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://knm.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyw.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bei.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uku.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wve.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uct.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fvq.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://vbr.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kqe.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kzg.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ows.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bes.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cwn.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dem.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://seb.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zsc.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://uau.hnqzz.top

Py:   resp.json()
来源：http://gbi.uphjek.com

PHP:  json_decode($body, true);
来源：http://ogf.hysaishi.cn

JS:   await resp.json()
来源：http://mck.hywenlv.cn

TS:   await resp.json()
来源：http://tak.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bcw.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jqp.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://bud.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lop.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://yyx.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dgc.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ylu.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://uks.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://ixl.daria6918.cn

Java: resp.statusCode()
来源：http://nze.vqdsnc.cn

Go:   resp.StatusCode
来源：http://zrr.sweek.top

Ruby: resp.code.to_i
来源：http://onn.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://xrl.xylfe.cn

[L08] 并发请求多个地址
来源：http://fgb.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfq.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://dre.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzj.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pne.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hic.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cdw.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://llh.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wia.sjlbkw.cn

================================================================================
来源：http://ntr.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://qhq.yanxiufei.cn

================================================================================
来源：http://uiu.316326.xyz

[M01] 读取命令行参数
来源：http://fbc.daria6918.cn

Py:   sys.argv[1:]
来源：http://fxl.aizwys.cn

PHP:  $argv;  $argc;
来源：http://ptf.birdmap.top

JS:   process.argv.slice(2)
来源：http://tgy.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://dsi.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://blb.xuanzx.com

Go:   os.Args[1:]
来源：http://thk.fktsv.cn

Ruby: ARGV
来源：http://bog.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://sxl.nwbrower.top

[M02] 读取环境变量
来源：http://rnb.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://ijj.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpb.zhixingplan.top

JS:   process.env.HOME
来源：http://udp.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://cpo.zdbjq.cn

Java: System.getenv("HOME")
来源：http://hul.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xgp.cucudq.cn

Ruby: ENV["HOME"]
来源：http://jhm.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnt.hnxiangtu.top

[M03] 执行外部命令
来源：http://vjs.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uja.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owf.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lyq.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jxw.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://syr.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fkn.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://ian.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://dxi.316326.xyz

[M04] 获取当前工作目录
来源：http://ges.hywenlv.cn

Py:   os.getcwd()
来源：http://lvq.yonumen.top

PHP:  getcwd();
来源：http://pxo.zdbjq.cn

JS:   process.cwd()
来源：http://xmc.gogol.net.cn

TS:   process.cwd()
来源：http://sbh.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://zhg.redwolf501.top

Go:   os.Getwd()
来源：http://wnj.fktsv.cn

Ruby: Dir.pwd
来源：http://pul.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://yly.ctjpmb.com

[M05] 设置退出码
来源：http://waq.sxryk.cn

Py:   sys.exit(1)
来源：http://cnv.tanke756.top

PHP:  exit(1);
来源：http://gvf.zhijiandao.cn

JS:   process.exit(1)
来源：http://jkl.chenjidiqi.icu

TS:   process.exit(1)
来源：http://szo.jinqigufen.top

Java: System.exit(1)
来源：http://wyi.wangdashe.top

Go:   os.Exit(1)
来源：http://tse.zhaomingkeji.xyz

Ruby: exit 1
来源：http://qtb.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tfd.hfpthk.cn

[M06] 向标准错误输出
来源：http://ujs.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://xyv.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vih.hesvh.cn

JS:   console.error("err")
来源：http://rue.cqqwz.cn

TS:   console.error("err")
来源：http://lsr.meibo888.top

Java: System.err.println("err")
来源：http://had.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://woz.pycfn.com

Ruby: warn "err"
来源：http://kkr.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://qur.daria6918.cn

[M07] 判断是否为主入口
来源：http://ndw.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://hwl.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ula.ywan-chungtsiang.top

JS:   require.main === module
来源：http://rhh.pengpengdd.cyou

TS:   require.main === module
来源：http://gob.nwbrower.top

Java: public static void main(String[] args)
来源：http://jnv.bbcook.cn

Go:   func main()
来源：http://kqe.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fnu.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://cju.tanke756.top

[M08] 获取系统与运行时信息
来源：http://qap.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://nas.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://zia.mhx1999.top

JS:   process.platform;  process.version
来源：http://pan.tanke756.top

TS:   process.platform;  process.version
来源：http://zxc.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cvk.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gje.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://twb.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://alk.sufxvd.cn

================================================================================
来源：http://ulk.ehwqpu.com

N. 数据结构与算法
来源：http://tkw.guowangkeji.top

================================================================================
来源：http://wqo.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://tjb.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://zhj.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ykv.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcn.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfk.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://iej.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://seo.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wfg.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://eia.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wfa.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://dys.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vjz.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jna.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hrp.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emn.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://ilj.vqdsnc.cn

Ruby: arr.sort
来源：http://qhl.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xti.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://zjw.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fhs.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://hat.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nrc.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ruj.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gbv.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xie.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dgs.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bcz.nanxinkj.top

[N04] 斐波那契数列
来源：http://uln.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ddx.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cip.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://anc.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tzg.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aeb.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://foc.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cyy.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fbu.vqdsnc.cn

[N05] 最大公约数
来源：http://deu.nwbrower.top

Py:   math.gcd(a, b)
来源：http://ggs.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ydq.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cfr.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okc.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hdf.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wju.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://yqs.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mrj.bjfxy.top

[N06] 判断回文字符串
来源：http://gts.smart0.xyz

Py:   s == s[::-1]
来源：http://tgb.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://miw.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://abs.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://ntx.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ohq.sysykeji.top

Go:   // 双指针从两端比较
来源：http://gej.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://sne.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zre.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://pbk.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tmf.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ofl.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ldw.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://rjd.cucudq.cn

Java: // 手写 HashMap
来源：http://gqk.mhx1999.top

Go:   // 手写 map[int]int
来源：http://gbk.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://osa.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://hia.haohaochexian.top

[N08] 生成全排列
来源：http://cml.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://flc.jianghu66.top

PHP:  // 手写递归交换
来源：http://pgf.shuidangran.top

JS:   // 手写回溯递归
来源：http://vwn.haohaochexian.top

TS:   // 手写回溯递归
来源：http://ybh.sysykeji.top

Java: // 手写回溯递归
来源：http://mrg.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://soz.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://fvt.wangdashe.top

C#:   // 手写回溯递归
来源：http://hwb.tian-w.cn

[N09] 栈与队列
来源：http://gwg.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pny.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oqv.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pux.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lyx.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nnu.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zjp.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://apy.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tqo.hongshengwenyu.top

[N10] 链表节点定义
来源：http://csj.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ztz.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gxg.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qck.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nbr.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://wdg.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://arm.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pzx.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fyw.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://pqx.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lez.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://ylb.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wcu.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hfw.xuetiantiany.cn

Java: // 手写递归
来源：http://ncl.zdbjq.cn

Go:   // 手写递归
来源：http://rrf.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zng.sweek.top

C#:   // 手写递归
来源：http://uuy.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cmv.52xcode.cn


<!-- 参考信息 -->