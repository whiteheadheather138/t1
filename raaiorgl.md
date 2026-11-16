代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://fgp.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hgm.c1oappe.top

[K04] 读取 JSON 文件
来源：http://rcc.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jnq.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pei.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://org.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dqn.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cdn.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lhk.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://uym.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxd.nanxuanxn.top

[K05] 深拷贝对象
来源：http://fyg.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://njc.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://lnd.cashguo.top

JS:   structuredClone(obj)
来源：http://atk.havefunace.top

TS:   structuredClone(obj)
来源：http://xda.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://thj.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://csn.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oaf.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://fof.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://yov.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kkp.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pmv.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uis.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nlc.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dsh.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvr.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uyf.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vow.gzhubu.top

[K07] 进制转换
来源：http://qpc.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vji.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jye.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xxk.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uck.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://foe.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rtv.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ecq.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qvp.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://mgv.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://edg.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ojx.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://luj.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://pon.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tdo.hnqzz.top

Go:   encoding/gob
来源：http://ljb.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://pkv.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://itz.zhiwuduotai.top

================================================================================
来源：http://ftf.ehwqpu.com

L. 网络请求
来源：http://wgj.cheryme.top

================================================================================
来源：http://liz.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://eyo.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://old.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mqk.bbcook.cn

JS:   await fetch(url)
来源：http://tlc.0kj1m.cn

TS:   await fetch(url)
来源：http://zlr.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bbk.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://geq.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hpk.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ncb.yj20258.top

[L02] 发送 POST JSON
来源：http://ugv.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://iml.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iul.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skt.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aev.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dkk.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://crc.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gui.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ada.tianlin.xyz

[L03] 设置自定义请求头
来源：http://vjd.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pok.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qxw.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://otc.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckq.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfw.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lym.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hxm.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jsx.havefunace.top

[L04] 设置超时
来源：http://lli.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://yzn.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://txt.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://csq.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwr.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ven.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lhs.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxt.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sph.yj20258888.top

[L05] 上传文件（multipart）
来源：http://yoi.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lel.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qug.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ixj.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://thg.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uka.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://asb.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dvx.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kkm.yonumen.top

[L06] 解析响应为 JSON
来源：http://fnf.cheryme.top

Py:   resp.json()
来源：http://izz.yongpay.top

PHP:  json_decode($body, true);
来源：http://nlk.uphjek.com

JS:   await resp.json()
来源：http://xfx.fzhhl.top

TS:   await resp.json()
来源：http://yqc.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pkj.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lwt.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://wwf.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rnf.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://eco.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://llj.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ggy.yj202588.top

JS:   resp.ok;  resp.status
来源：http://jlk.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://jzz.guannengcc.top

Java: resp.statusCode()
来源：http://zlr.sufxvd.cn

Go:   resp.StatusCode
来源：http://ggr.hnqzz.top

Ruby: resp.code.to_i
来源：http://qpg.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://sxb.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://zlq.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xrd.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://bxz.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnj.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://afg.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yoy.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ncs.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hdj.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmy.yj202588.top

================================================================================
来源：http://gjl.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://vks.jyoumei.cn

================================================================================
来源：http://cpc.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://hvu.nanxinkj.top

Py:   sys.argv[1:]
来源：http://kcz.xziqi.cn

PHP:  $argv;  $argc;
来源：http://txa.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://aie.ybcxt.top

TS:   process.argv.slice(2)
来源：http://yzb.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://ckp.cqqwz.cn

Go:   os.Args[1:]
来源：http://ixe.cdnleiting.top

Ruby: ARGV
来源：http://xws.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://xyv.jyoumei.cn

[M02] 读取环境变量
来源：http://smq.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://oqn.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wyj.hcnkem.com

JS:   process.env.HOME
来源：http://dyy.gotoacloud.top

TS:   process.env.HOME
来源：http://dnb.hysaishi.cn

Java: System.getenv("HOME")
来源：http://jsk.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vhz.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://exg.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gpq.meibo888.top

[M03] 执行外部命令
来源：http://uxt.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bsa.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qun.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lts.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oan.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://obk.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dgt.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://seo.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://yei.shzxlz.cn

[M04] 获取当前工作目录
来源：http://sqs.fzhhl.top

Py:   os.getcwd()
来源：http://mpd.52xcode.cn

PHP:  getcwd();
来源：http://szh.gogol.net.cn

JS:   process.cwd()
来源：http://jnc.xuetiantiany.cn

TS:   process.cwd()
来源：http://mux.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://rcj.fzhhl.top

Go:   os.Getwd()
来源：http://oqr.jinqigufen.top

Ruby: Dir.pwd
来源：http://bht.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://wrs.shangyingyoupin.top

[M05] 设置退出码
来源：http://mtw.svipenyu.cn

Py:   sys.exit(1)
来源：http://als.quarkkingdee.top

PHP:  exit(1);
来源：http://tpx.bjfxy.top

JS:   process.exit(1)
来源：http://wew.jiagoushi.top

TS:   process.exit(1)
来源：http://ptm.ehwqpu.com

Java: System.exit(1)
来源：http://pie.zhengqikj.top

Go:   os.Exit(1)
来源：http://iot.pengpengdd.cyou

Ruby: exit 1
来源：http://jfj.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xqu.vehdjk.com

[M06] 向标准错误输出
来源：http://zlf.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://zwc.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gup.fanxiaobao.xyz

JS:   console.error("err")
来源：http://rpu.hywenlv.cn

TS:   console.error("err")
来源：http://fon.cashguo.top

Java: System.err.println("err")
来源：http://znd.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zjs.hnxiangtu.top

Ruby: warn "err"
来源：http://xyw.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://wqm.sxryk.cn

[M07] 判断是否为主入口
来源：http://izn.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://pbh.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bcq.cashguo.top

JS:   require.main === module
来源：http://ltq.wangdashe.top

TS:   require.main === module
来源：http://gzk.meibo888.top

Java: public static void main(String[] args)
来源：http://ata.tian-w.cn

Go:   func main()
来源：http://zrb.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fcg.yj20258888.top

C#:   static void Main(string[] args)
来源：http://zcz.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://gju.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://mep.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://sex.havefunace.top

JS:   process.platform;  process.version
来源：http://wrt.bjfxy.top

TS:   process.platform;  process.version
来源：http://mjy.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxz.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xqe.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzu.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://srl.jinqigfzy.top

================================================================================
来源：http://gnt.zhixingplan.top

N. 数据结构与算法
来源：http://syo.vehdjk.com

================================================================================
来源：http://mkq.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://cdc.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uzb.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://etu.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://awu.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnu.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://fuk.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://bvi.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyf.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://tcw.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://jqy.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://zsx.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gai.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iam.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sew.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kkk.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://rfv.guannengcc.top

Ruby: arr.sort
来源：http://xmm.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyj.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://jpx.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lbl.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://ugc.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qwy.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zds.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ngu.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ezd.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xau.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://bbs.jqgfzy.top

[N04] 斐波那契数列
来源：http://rey.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uvp.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ncf.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdm.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fss.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trk.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dpx.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pxo.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovl.fktsv.cn

[N05] 最大公约数
来源：http://ccq.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://dtd.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dec.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdv.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqu.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cys.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://geq.9152youxi.cn

Ruby: a.gcd(b)
来源：http://rmt.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iwh.jinqigfzy.top

[N06] 判断回文字符串
来源：http://oef.ybcxt.top

Py:   s == s[::-1]
来源：http://xjr.sxryk.cn

PHP:  $s === strrev($s);
来源：http://mnl.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://jvk.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://bcs.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gsf.zycfv.cn

Go:   // 双指针从两端比较
来源：http://ypi.jqgfzy.top

Ruby: s == s.reverse
来源：http://sbx.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://dcs.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://shp.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nsj.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hbj.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iqy.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://gft.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://upe.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://fnk.yongpay.top

Ruby: // 手写 Hash
来源：http://nek.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sew.zhengqikj.top

[N08] 生成全排列
来源：http://izv.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://bhg.ehwqpu.com

PHP:  // 手写递归交换
来源：http://btp.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://nmm.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://swn.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://yfs.zdbjq.cn

Go:   // 手写回溯递归
来源：http://vjm.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://olb.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://yun.yongpay.top

[N09] 栈与队列
来源：http://usm.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kys.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ufi.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dar.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zmo.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ydv.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cmu.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://svu.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zse.epnwcf.com

[N10] 链表节点定义
来源：http://rby.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://crh.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nbl.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mqi.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://liq.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://dlc.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uij.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xfv.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://miz.yongpay.top

[N11] 二叉树中序遍历
来源：http://jwr.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oou.cdnleiting.top

PHP:  // 手写递归函数
来源：http://pne.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zjf.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byw.hesvh.cn

Java: // 手写递归
来源：http://rtv.jiagoushi.top

Go:   // 手写递归
来源：http://ilh.fktsv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lsp.sxryk.cn

C#:   // 手写递归
来源：http://xdk.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yaa.gzhubu.top


<!-- 参考信息 -->