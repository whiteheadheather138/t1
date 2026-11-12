代发 wailian999

[K02] JSON 字符串转对象
来源：http://tpw.cheryme.top

Py:   json.loads(s)
来源：http://mgx.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nyd.yfazqb.com

JS:   JSON.parse(s)
来源：http://cqo.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://iik.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dxv.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://qtc.bbcook.cn

Ruby: JSON.parse(s)
来源：http://ojy.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qwg.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://gak.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vwi.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yqk.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kdw.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://esw.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rjq.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gkc.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://urv.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lkh.ydzc1.top

[K04] 读取 JSON 文件
来源：http://ihd.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnj.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iqv.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrg.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://naj.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rnq.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://saj.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kot.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dbg.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://vnq.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://lmu.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://qqs.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://xhp.haohaochexian.top

TS:   structuredClone(obj)
来源：http://usi.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ezo.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kyd.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://atp.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://upw.hesvh.cn

[K06] 解析 URL 查询串
来源：http://qck.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://imp.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qto.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://buo.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jig.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qhj.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hmr.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yeq.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bjr.dianchejie.cn

[K07] 进制转换
来源：http://doh.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ipd.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ado.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vfv.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rws.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iup.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uaa.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ctt.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bus.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://shd.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://bdp.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ouo.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://kte.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://cmy.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://chj.nanxuanxn.top

Go:   encoding/gob
来源：http://uct.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://xue.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://chb.cashguo.top

================================================================================
来源：http://zbn.feifeiyinyue.top

L. 网络请求
来源：http://vjq.52xcode.cn

================================================================================
来源：http://vwg.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://uro.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cgu.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gdx.hysaishi.cn

JS:   await fetch(url)
来源：http://cgu.zdqjudy.top

TS:   await fetch(url)
来源：http://rkd.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zep.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://vbl.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://dbu.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://scb.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://arw.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://icp.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://frs.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bva.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://elp.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qfs.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aoq.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mpx.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jcq.aibaodan.cn

[L03] 设置自定义请求头
来源：http://yyd.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tsw.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zra.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bau.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwb.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rel.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wvm.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://klr.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vdx.yfazqb.com

[L04] 设置超时
来源：http://lpn.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://wbx.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgo.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxo.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mpr.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jig.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://box.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yfx.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ots.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://htp.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zko.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qun.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lei.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfl.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bus.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kws.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://clg.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tfp.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://llt.zhijiandao.cn

Py:   resp.json()
来源：http://wnl.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://kfq.yongpay.top

JS:   await resp.json()
来源：http://qnt.redwolf501.top

TS:   await resp.json()
来源：http://vki.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qap.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://moo.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://acv.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yha.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://ejb.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itw.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fnw.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://prm.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://nmi.jqgfzy.top

Java: resp.statusCode()
来源：http://prb.snrcjt.cn

Go:   resp.StatusCode
来源：http://jbh.fengsongda.top

Ruby: resp.code.to_i
来源：http://rdv.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://zzd.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://oaw.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yme.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://vqg.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xdc.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxp.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://acs.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ogg.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rnl.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://csj.sysykeji.top

================================================================================
来源：http://mgu.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://gfy.havefunace.top

================================================================================
来源：http://jnu.ydjk.org.cn

[M01] 读取命令行参数
来源：http://klc.uphjek.com

Py:   sys.argv[1:]
来源：http://xhv.hesvh.cn

PHP:  $argv;  $argc;
来源：http://xak.52xcode.cn

JS:   process.argv.slice(2)
来源：http://deu.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://mag.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://rwp.yj20258.top

Go:   os.Args[1:]
来源：http://heo.fanxiaobao.xyz

Ruby: ARGV
来源：http://edt.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://dip.yuanzhike.top

[M02] 读取环境变量
来源：http://cxa.cheryme.top

Py:   os.environ.get("HOME")
来源：http://hin.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hpm.nanxinkj.top

JS:   process.env.HOME
来源：http://zxa.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://tpp.zhengqikj.top

Java: System.getenv("HOME")
来源：http://omk.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ijs.uphjek.com

Ruby: ENV["HOME"]
来源：http://vrd.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ybe.52xcode.cn

[M03] 执行外部命令
来源：http://poo.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qui.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lgc.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bxe.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xae.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gan.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zqb.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zww.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://sgk.tanke756.top

[M04] 获取当前工作目录
来源：http://mag.dashuyun.cn

Py:   os.getcwd()
来源：http://vut.hongshengwenyu.top

PHP:  getcwd();
来源：http://vbm.pengpengdd.cyou

JS:   process.cwd()
来源：http://fhe.bbcook.cn

TS:   process.cwd()
来源：http://mhr.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://pmy.dashuyun.cn

Go:   os.Getwd()
来源：http://mia.cashguo.top

Ruby: Dir.pwd
来源：http://pez.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fed.gzhubu.top

[M05] 设置退出码
来源：http://ros.daria6918.cn

Py:   sys.exit(1)
来源：http://maz.snrcjt.cn

PHP:  exit(1);
来源：http://gjg.mhx1999.top

JS:   process.exit(1)
来源：http://hpb.zhijiandao.cn

TS:   process.exit(1)
来源：http://adx.fzhhl.top

Java: System.exit(1)
来源：http://kwl.havefunace.top

Go:   os.Exit(1)
来源：http://gtn.hesvh.cn

Ruby: exit 1
来源：http://iqu.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://loy.shuidangran.top

[M06] 向标准错误输出
来源：http://jzu.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://cim.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://brt.jqgufenzy.top

JS:   console.error("err")
来源：http://ynf.sufxvd.cn

TS:   console.error("err")
来源：http://fse.yfazqb.com

Java: System.err.println("err")
来源：http://zcg.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gek.zhongyouzk.top

Ruby: warn "err"
来源：http://ydf.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://nkk.xinyue.icu

[M07] 判断是否为主入口
来源：http://mxl.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://awb.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zaj.hesvh.cn

JS:   require.main === module
来源：http://eru.aizwys.cn

TS:   require.main === module
来源：http://fkz.birdmap.top

Java: public static void main(String[] args)
来源：http://qgk.ppjwa.cn

Go:   func main()
来源：http://dyq.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mae.vehdjk.com

C#:   static void Main(string[] args)
来源：http://hol.ivvv.top

[M08] 获取系统与运行时信息
来源：http://cqk.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://xaf.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://ntt.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://byk.sysykeji.top

TS:   process.platform;  process.version
来源：http://yiq.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://use.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ddv.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aml.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmg.hcnkem.com

================================================================================
来源：http://pap.zhengqikj.top

N. 数据结构与算法
来源：http://psn.havefunace.top

================================================================================
来源：http://zdv.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://jkr.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ucn.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fso.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzy.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwq.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://cyd.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://btb.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fyt.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gsf.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://rqi.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://ruv.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oxg.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yow.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mmq.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qqa.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://azb.vqdsnc.cn

Ruby: arr.sort
来源：http://slc.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://sns.tarul.cn

[N03] 快速排序（分治示例）
来源：http://lwy.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cgh.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://skm.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jzy.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vst.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://atz.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bas.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xkt.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ngu.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://bkg.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iel.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://arc.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ypy.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lww.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ful.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bea.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ism.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ykr.zhongyouzk.top

[N05] 最大公约数
来源：http://mnk.andypj.xyz

Py:   math.gcd(a, b)
来源：http://pgw.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ffq.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jmx.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yuj.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oxh.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jws.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://rzd.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ppn.ydjk.org.cn

[N06] 判断回文字符串
来源：http://oaa.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://mus.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://rmm.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://hba.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://uux.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lqn.cucudq.cn

Go:   // 双指针从两端比较
来源：http://sur.zhongyouzk.top

Ruby: s == s.reverse
来源：http://gdp.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfx.316326.xyz

[N07] 两数之和（返回下标）
来源：http://blv.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pxc.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yrq.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gih.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://dop.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://grs.tian-w.cn

Go:   // 手写 map[int]int
来源：http://pda.epnwcf.com

Ruby: // 手写 Hash
来源：http://slm.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://mic.yongpay.top

[N08] 生成全排列
来源：http://kiq.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://kte.cucudq.cn

PHP:  // 手写递归交换
来源：http://mfz.yj202588.top

JS:   // 手写回溯递归
来源：http://mla.fktsv.cn

TS:   // 手写回溯递归
来源：http://wcm.zhengqikj.top

Java: // 手写回溯递归
来源：http://igo.xuanzx.com

Go:   // 手写回溯递归
来源：http://vyl.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://mwt.birdmap.top

C#:   // 手写回溯递归
来源：http://sqq.sjlbkw.cn

[N09] 栈与队列
来源：http://kns.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mke.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iey.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zqa.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aku.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tro.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://obw.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://piw.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wzf.zhoulong.xyz

[N10] 链表节点定义
来源：http://exy.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lny.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://shp.0kj1m.cn


<!-- 参考信息 -->