代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iqm.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://uoi.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oym.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hip.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kvr.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qwu.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dzq.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nmo.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://dod.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uod.yueranfly.top

[K04] 读取 JSON 文件
来源：http://swh.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rqz.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pfh.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ckq.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qpy.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tcx.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tui.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wwp.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iou.hammf.cn

[K05] 深拷贝对象
来源：http://ydf.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://rqz.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://dcp.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://sdl.yonumen.top

TS:   structuredClone(obj)
来源：http://tfd.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xso.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yrj.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jyg.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://biq.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://lco.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gmm.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eqd.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfw.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppp.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://koo.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kyh.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qms.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ise.jinyuanbaomall.cn

[K07] 进制转换
来源：http://osk.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rlz.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bhe.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ltc.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qiz.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://you.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gta.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oea.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fof.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://cea.pycfn.com

Py:   pickle.dumps(obj)
来源：http://tja.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kul.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://gug.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://gul.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lst.cqqwz.cn

Go:   encoding/gob
来源：http://ldo.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://rsv.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://otn.nwbrower.top

================================================================================
来源：http://cpl.yvedp.cn

L. 网络请求
来源：http://ize.yj202588.top

================================================================================
来源：http://tvp.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://hrk.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wzk.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wel.c1oappe.top

JS:   await fetch(url)
来源：http://fqi.ehwqpu.com

TS:   await fetch(url)
来源：http://ash.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rju.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://zvz.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jgl.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://smn.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://ecl.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://cfc.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yld.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzo.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eib.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wiy.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jjh.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dqs.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vqg.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://nxu.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ofx.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sol.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kes.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://swp.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ngp.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lmb.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://icw.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cqk.zdbjq.cn

[L04] 设置超时
来源：http://vug.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://zms.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uce.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rss.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzm.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://khg.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zjn.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kvb.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xip.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://trb.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jtc.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eqv.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lnj.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iem.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tbq.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://omg.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxb.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oze.hcnkem.com

[L06] 解析响应为 JSON
来源：http://wmj.quarkkingdee.top

Py:   resp.json()
来源：http://ylj.jianghu66.top

PHP:  json_decode($body, true);
来源：http://dyr.yfazqb.com

JS:   await resp.json()
来源：http://yib.pengpengdd.cyou

TS:   await resp.json()
来源：http://cji.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vkt.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bfa.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://lzo.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kau.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://wnr.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hkj.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ngu.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://nsu.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://mlw.cheryme.top

Java: resp.statusCode()
来源：http://riy.dashuyun.cn

Go:   resp.StatusCode
来源：http://xfy.snrcjt.cn

Ruby: resp.code.to_i
来源：http://tke.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://ieu.c1oappe.top

[L08] 并发请求多个地址
来源：http://drx.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kxd.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://oei.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gdd.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzm.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rrx.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dye.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fyc.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mau.yangfankeji.com

================================================================================
来源：http://ayd.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://xrf.gogol.net.cn

================================================================================
来源：http://mti.bbcook.cn

[M01] 读取命令行参数
来源：http://jxg.iojbl.cn

Py:   sys.argv[1:]
来源：http://bil.xuanzx.com

PHP:  $argv;  $argc;
来源：http://zfg.iojbl.cn

JS:   process.argv.slice(2)
来源：http://dhu.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://ita.uphjek.com

Java: args 数组（main 方法参数）
来源：http://ggx.epnwcf.com

Go:   os.Args[1:]
来源：http://mll.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://xnh.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://lat.xinyue.icu

[M02] 读取环境变量
来源：http://caj.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://kbu.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyn.ppjwa.cn

JS:   process.env.HOME
来源：http://dsx.guannengcc.top

TS:   process.env.HOME
来源：http://yte.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://mup.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ewn.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://ikl.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rju.gogol.net.cn

[M03] 执行外部命令
来源：http://pij.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzd.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xem.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sdh.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ktf.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://thy.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://msr.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://quv.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://uji.hnqzz.top

[M04] 获取当前工作目录
来源：http://tlm.sjlbkw.cn

Py:   os.getcwd()
来源：http://kti.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://oao.fengsongda.top

JS:   process.cwd()
来源：http://tjx.andypj.xyz

TS:   process.cwd()
来源：http://lji.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://ial.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://chb.tarul.cn

Ruby: Dir.pwd
来源：http://pjf.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jjl.cqqwz.cn

[M05] 设置退出码
来源：http://mmx.nanxinkj.top

Py:   sys.exit(1)
来源：http://abe.yuxming.cn

PHP:  exit(1);
来源：http://oty.zhoulong.xyz

JS:   process.exit(1)
来源：http://xyi.zhengqikj.top

TS:   process.exit(1)
来源：http://izn.tarul.cn

Java: System.exit(1)
来源：http://xle.52xcode.cn

Go:   os.Exit(1)
来源：http://nhk.havefunace.top

Ruby: exit 1
来源：http://iyj.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xph.yj20258.top

[M06] 向标准错误输出
来源：http://tmg.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://qfu.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://tdv.yfazqb.com

JS:   console.error("err")
来源：http://nwk.cucudq.cn

TS:   console.error("err")
来源：http://vtf.zdbjq.cn

Java: System.err.println("err")
来源：http://iij.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://viq.jinghuilouyu.cn

Ruby: warn "err"
来源：http://ftf.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://tqb.cashguo.top

[M07] 判断是否为主入口
来源：http://dya.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://nix.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yit.zdbjq.cn

JS:   require.main === module
来源：http://zuz.yonumen.top

TS:   require.main === module
来源：http://tew.sweek.top

Java: public static void main(String[] args)
来源：http://bpu.fengsongda.top

Go:   func main()
来源：http://ffy.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kkx.yj202588.top

C#:   static void Main(string[] args)
来源：http://qld.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://bgz.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://msk.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://coo.cqqwz.cn

JS:   process.platform;  process.version
来源：http://jmm.zdbjq.cn

TS:   process.platform;  process.version
来源：http://vtu.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dvm.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zwk.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vtg.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lnp.zycfv.cn

================================================================================
来源：http://jrz.epnwcf.com

N. 数据结构与算法
来源：http://rbe.redwolf501.top

================================================================================
来源：http://yzl.birdmap.top

[N01] 二分查找（有序数组）
来源：http://sjy.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://plm.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ztu.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://umx.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcm.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lsw.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://sgk.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eqh.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zqh.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://tve.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://ked.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tin.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oea.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vln.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coh.yvedp.cn

Go:   slices.Sort(arr)
来源：http://rnd.sjlbkw.cn

Ruby: arr.sort
来源：http://nti.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tkt.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://vpd.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://afh.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://fby.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wyp.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sci.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://psw.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uti.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nzg.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://qvx.zhixingplan.top

[N04] 斐波那契数列
来源：http://tdo.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://osq.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xmq.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wkq.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvb.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hzf.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ast.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://prg.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://adv.chenzaomai.com

[N05] 最大公约数
来源：http://clh.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://rnl.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvb.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgu.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zzd.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vmo.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rgw.tianlin.xyz

Ruby: a.gcd(b)
来源：http://hfr.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uxa.ppjwa.cn

[N06] 判断回文字符串
来源：http://fbm.sjlbkw.cn

Py:   s == s[::-1]
来源：http://jea.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://wzz.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://gxe.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://was.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fve.yj20258.top

Go:   // 双指针从两端比较
来源：http://jjc.cucudq.cn

Ruby: s == s.reverse
来源：http://sbs.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vrh.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://dem.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://huo.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://anl.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ayu.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://fqm.9152youxi.cn

Java: // 手写 HashMap
来源：http://qqq.bjfxy.top

Go:   // 手写 map[int]int
来源：http://enr.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://fti.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://ubn.epnwcf.com

[N08] 生成全排列
来源：http://bgd.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://ova.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://qkf.haohaochexian.top

JS:   // 手写回溯递归
来源：http://rdb.zycfv.cn

TS:   // 手写回溯递归
来源：http://dyj.guowangkeji.top

Java: // 手写回溯递归
来源：http://gup.zhixingplan.top

Go:   // 手写回溯递归
来源：http://ooz.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://oys.dashuyun.cn

C#:   // 手写回溯递归
来源：http://jth.yfazqb.com

[N09] 栈与队列
来源：http://qeu.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qbu.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mev.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pwe.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xwt.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blu.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dec.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ucf.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mux.tanke756.top

[N10] 链表节点定义
来源：http://sio.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbm.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://efc.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hun.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ync.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://zjf.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://ygo.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ifb.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ulq.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://xnv.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qsi.cqqwz.cn


<!-- 参考信息 -->