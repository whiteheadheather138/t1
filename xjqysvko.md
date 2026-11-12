代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://pcw.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ded.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://xul.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgz.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yog.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sqy.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ulc.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jak.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oms.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://avi.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xfo.yfazqb.com

[K05] 深拷贝对象
来源：http://arv.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://cjx.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://cbz.xinyue.icu

JS:   structuredClone(obj)
来源：http://rbj.yfazqb.com

TS:   structuredClone(obj)
来源：http://mfg.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vqj.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gcn.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdw.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://epi.tarul.cn

[K06] 解析 URL 查询串
来源：http://eqx.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pva.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fgm.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mlj.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ipe.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ydp.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fqk.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gex.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ynu.zhixingplan.top

[K07] 进制转换
来源：http://igo.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sst.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zft.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vcc.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://stq.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nyo.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jaf.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ibu.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xgl.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://wfc.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://qyc.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://swo.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://lnm.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://xli.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dop.gzhubu.top

Go:   encoding/gob
来源：http://loa.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://vum.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aoy.ppjwa.cn

================================================================================
来源：http://fov.zhixingplan.top

L. 网络请求
来源：http://poa.sufxvd.cn

================================================================================
来源：http://jpo.wangdashe.top

[L01] 发送 GET 请求
来源：http://jin.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mlr.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://upj.yonumen.top

JS:   await fetch(url)
来源：http://pau.bjfxy.top

TS:   await fetch(url)
来源：http://bbj.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://puz.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://fwf.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jal.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tbv.cqqwz.cn

[L02] 发送 POST JSON
来源：http://ezd.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://yio.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfn.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wlo.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qfx.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfc.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eos.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ybn.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oeu.uphjek.com

[L03] 设置自定义请求头
来源：http://cgz.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ejf.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pkm.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpf.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hix.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hgv.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lzq.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kzt.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hno.zhongyouzk.top

[L04] 设置超时
来源：http://yvh.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://wbq.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fqm.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgl.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhr.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyd.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgb.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://omq.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nis.smart0.xyz

[L05] 上传文件（multipart）
来源：http://rst.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rqb.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wrr.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kcu.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gqd.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fxy.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jft.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtl.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aps.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://vob.fzhhl.top

Py:   resp.json()
来源：http://thk.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://pqb.andypj.xyz

JS:   await resp.json()
来源：http://iap.uphjek.com

TS:   await resp.json()
来源：http://fkv.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kik.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hca.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://tdj.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fsw.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://tyi.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kgn.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svf.havefunace.top

JS:   resp.ok;  resp.status
来源：http://yre.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://xeh.zhengqikj.top

Java: resp.statusCode()
来源：http://zlf.sxryk.cn

Go:   resp.StatusCode
来源：http://wnk.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://itv.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://jbk.shuidangran.top

[L08] 并发请求多个地址
来源：http://fzg.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://suj.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://ytk.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzx.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdd.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vow.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ugg.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uyc.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ict.cheryme.top

================================================================================
来源：http://sqq.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://xed.ehwqpu.com

================================================================================
来源：http://lpq.kuanghao11.cn

[M01] 读取命令行参数
来源：http://eve.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://rfj.hnqzz.top

PHP:  $argv;  $argc;
来源：http://qii.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://fux.yj202588.top

TS:   process.argv.slice(2)
来源：http://zox.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://lwz.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://vrn.ydjk.org.cn

Ruby: ARGV
来源：http://ffh.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://zli.yj202588.top

[M02] 读取环境变量
来源：http://chj.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://zyr.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vlj.snrcjt.cn

JS:   process.env.HOME
来源：http://hcy.cheryme.top

TS:   process.env.HOME
来源：http://jqh.svipenyu.cn

Java: System.getenv("HOME")
来源：http://gmj.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dcy.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://ojv.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pxk.yuanzhike.top

[M03] 执行外部命令
来源：http://hxl.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tea.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sgs.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://acy.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://haq.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://urm.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nsr.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://nax.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://vhe.gogol.net.cn

[M04] 获取当前工作目录
来源：http://jjb.hywenlv.cn

Py:   os.getcwd()
来源：http://alm.vqdsnc.cn

PHP:  getcwd();
来源：http://osb.guowangkeji.top

JS:   process.cwd()
来源：http://ept.jqgfzy.top

TS:   process.cwd()
来源：http://ulk.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://rin.shzxlz.cn

Go:   os.Getwd()
来源：http://tmw.hcnkem.com

Ruby: Dir.pwd
来源：http://gbm.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://qpv.snrcjt.cn

[M05] 设置退出码
来源：http://mon.guowangkeji.top

Py:   sys.exit(1)
来源：http://ajj.ybcxt.top

PHP:  exit(1);
来源：http://bty.aizwys.cn

JS:   process.exit(1)
来源：http://zan.yuxming.cn

TS:   process.exit(1)
来源：http://axv.fzhhl.top

Java: System.exit(1)
来源：http://bkl.tianlin.xyz

Go:   os.Exit(1)
来源：http://dfe.pengpengdd.cyou

Ruby: exit 1
来源：http://uce.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://obd.ivvv.top

[M06] 向标准错误输出
来源：http://ajq.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://bta.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lbz.tian-w.cn

JS:   console.error("err")
来源：http://fil.0kj1m.cn

TS:   console.error("err")
来源：http://duj.gaohongyu789.top

Java: System.err.println("err")
来源：http://bcn.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://npe.smart0.xyz

Ruby: warn "err"
来源：http://sbo.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://wpm.tianlin.xyz

[M07] 判断是否为主入口
来源：http://gvj.pycfn.com

Py:   if __name__ == "__main__":
来源：http://qom.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tts.redwolf501.top

JS:   require.main === module
来源：http://uij.chenlongwang.top

TS:   require.main === module
来源：http://sau.daxiang520.top

Java: public static void main(String[] args)
来源：http://vce.shangyingyoupin.top

Go:   func main()
来源：http://jrc.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ntf.jianghu66.top

C#:   static void Main(string[] args)
来源：http://dtf.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://xmq.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://few.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://hxb.yongpay.top

JS:   process.platform;  process.version
来源：http://lul.uphjek.com

TS:   process.platform;  process.version
来源：http://hty.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://crn.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hqf.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hux.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oal.shanyushiyangtech.top

================================================================================
来源：http://opl.ivvv.top

N. 数据结构与算法
来源：http://tvz.ppjwa.cn

================================================================================
来源：http://hwi.sweek.top

[N01] 二分查找（有序数组）
来源：http://kps.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kfx.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gby.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yvm.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oti.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://oge.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://kzz.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lxf.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://flx.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://cjg.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://nxn.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fvm.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fjc.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ocw.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cge.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://wia.shuidangran.top

Ruby: arr.sort
来源：http://vqw.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhb.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://ujd.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oaj.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://lqt.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lix.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jnk.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xdd.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xdu.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oig.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://zkm.daxiang520.top

[N04] 斐波那契数列
来源：http://mmf.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lzz.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bzz.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://adx.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ayq.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yhr.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xop.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hyq.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fqn.sweek.top

[N05] 最大公约数
来源：http://zop.jianghu66.top

Py:   math.gcd(a, b)
来源：http://gpc.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://juq.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jwt.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekd.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xng.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fbx.xinyue.icu

Ruby: a.gcd(b)
来源：http://rfw.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwo.quarkkingdee.top

[N06] 判断回文字符串
来源：http://rdq.hnxiangtu.top

Py:   s == s[::-1]
来源：http://aeg.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://ryd.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://knr.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://xdh.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cnu.havefunace.top

Go:   // 双指针从两端比较
来源：http://fbj.yfazqb.com

Ruby: s == s.reverse
来源：http://ngb.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cuw.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://ole.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ahd.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xej.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jib.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://otv.jianghu66.top

Java: // 手写 HashMap
来源：http://uvt.c1oappe.top

Go:   // 手写 map[int]int
来源：http://iix.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://vbz.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://zgk.hnxiangtu.top

[N08] 生成全排列
来源：http://htt.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://sqr.sxryk.cn

PHP:  // 手写递归交换
来源：http://evc.yonumen.top

JS:   // 手写回溯递归
来源：http://nbo.ctjpmb.com

TS:   // 手写回溯递归
来源：http://hum.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://nap.hysaishi.cn

Go:   // 手写回溯递归
来源：http://lmf.yj20258.top

Ruby: arr.permutation.to_a
来源：http://mql.yongpay.top

C#:   // 手写回溯递归
来源：http://cde.tianlin.xyz

[N09] 栈与队列
来源：http://oka.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rxb.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agy.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://stq.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tnk.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ptc.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tuj.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ofa.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://udb.0kj1m.cn

[N10] 链表节点定义
来源：http://nzh.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ope.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uyj.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ljy.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gxa.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://ybq.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://nyy.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uai.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ejo.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://chp.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eax.fengsongda.top

PHP:  // 手写递归函数
来源：http://qyp.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eja.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wit.fehbvm.com

Java: // 手写递归
来源：http://wyw.xylfe.cn

Go:   // 手写递归
来源：http://bss.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sir.zhijiandao.cn

C#:   // 手写递归
来源：http://oee.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wct.316326.xyz


<!-- 参考信息 -->