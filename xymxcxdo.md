代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zos.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://kcw.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xrs.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqt.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pxx.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vbe.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ldl.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nhu.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ddn.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://emn.sysykeji.top

[K04] 读取 JSON 文件
来源：http://gqn.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hvq.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rxt.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aic.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qhw.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lxb.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akz.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eeg.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ana.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://szo.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://wnd.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://hps.fktsv.cn

JS:   structuredClone(obj)
来源：http://ncu.yfazqb.com

TS:   structuredClone(obj)
来源：http://tnc.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mdg.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kjz.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ygi.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://kde.guannengcc.top

[K06] 解析 URL 查询串
来源：http://tzr.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gad.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pqq.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvb.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vac.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://klw.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fpz.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bda.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ely.cdnleiting.top

[K07] 进制转换
来源：http://fnu.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wye.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dht.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://swo.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ksr.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mrz.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vor.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mjw.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzb.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://hev.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://bux.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ndk.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://mca.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://muf.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yfe.gogol.net.cn

Go:   encoding/gob
来源：http://dxl.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://zdp.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hap.ppjwa.cn

================================================================================
来源：http://ika.nanxinkj.top

L. 网络请求
来源：http://nvc.fehbvm.com

================================================================================
来源：http://zrr.fzhhl.top

[L01] 发送 GET 请求
来源：http://mgm.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jua.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tuf.xinyue.icu

JS:   await fetch(url)
来源：http://iqs.redwolf501.top

TS:   await fetch(url)
来源：http://xfo.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nhh.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://ohw.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vps.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hvg.zdbjq.cn

[L02] 发送 POST JSON
来源：http://jwy.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://jgs.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rmg.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nfb.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bqj.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qam.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yuq.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://usa.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axs.hfpthk.cn

[L03] 设置自定义请求头
来源：http://kyd.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://whr.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tpi.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wxw.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hcy.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dkn.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://muq.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bvc.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqp.9152youxi.cn

[L04] 设置超时
来源：http://lwa.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://dfx.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hjc.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjs.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pwd.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://niq.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://enq.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jra.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xcm.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://jhw.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hlr.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nyo.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ous.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://boh.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wbx.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkr.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vrx.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nbr.cashguo.top

[L06] 解析响应为 JSON
来源：http://khw.kuanghao11.cn

Py:   resp.json()
来源：http://rbp.tanke756.top

PHP:  json_decode($body, true);
来源：http://tca.hnqzz.top

JS:   await resp.json()
来源：http://afx.yangfankeji.com

TS:   await resp.json()
来源：http://udr.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eqd.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ksb.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://nvi.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oja.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://cfs.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sdh.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqw.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://lju.birdmap.top

TS:   resp.ok;  resp.status
来源：http://yal.yfazqb.com

Java: resp.statusCode()
来源：http://kqs.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://aii.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://dzr.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://uka.pycfn.com

[L08] 并发请求多个地址
来源：http://mkh.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pcp.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://wtn.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyr.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwl.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pem.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fli.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfs.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sjv.316326.xyz

================================================================================
来源：http://gqr.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://ixq.bjfxy.top

================================================================================
来源：http://blz.9152youxi.cn

[M01] 读取命令行参数
来源：http://ffu.ivvv.top

Py:   sys.argv[1:]
来源：http://vhj.52xcode.cn

PHP:  $argv;  $argc;
来源：http://wss.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://zkp.andypj.xyz

TS:   process.argv.slice(2)
来源：http://ifv.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://nji.chenlongwang.top

Go:   os.Args[1:]
来源：http://lpq.yj202588.top

Ruby: ARGV
来源：http://uli.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://tfz.zhixingplan.top

[M02] 读取环境变量
来源：http://apm.uphjek.com

Py:   os.environ.get("HOME")
来源：http://zbr.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gaq.ydzc1.top

JS:   process.env.HOME
来源：http://lmq.gaohongyu789.top

TS:   process.env.HOME
来源：http://jhh.ctjpmb.com

Java: System.getenv("HOME")
来源：http://ylb.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rsv.xinyue.icu

Ruby: ENV["HOME"]
来源：http://izl.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hvd.xylfe.cn

[M03] 执行外部命令
来源：http://dla.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mkd.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ktr.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://asl.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ztq.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vrb.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ehh.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://nsi.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://huk.yangfankeji.com

[M04] 获取当前工作目录
来源：http://tdw.shuidangran.top

Py:   os.getcwd()
来源：http://uev.yanxiufei.cn

PHP:  getcwd();
来源：http://cvx.nanxuanxn.top

JS:   process.cwd()
来源：http://wnr.tarul.cn

TS:   process.cwd()
来源：http://sst.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://zqy.jianghu66.top

Go:   os.Getwd()
来源：http://poy.bbcook.cn

Ruby: Dir.pwd
来源：http://bdv.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://vnz.andypj.xyz

[M05] 设置退出码
来源：http://chl.hysaishi.cn

Py:   sys.exit(1)
来源：http://ncv.dianchejie.cn

PHP:  exit(1);
来源：http://yxp.nanxinkj.top

JS:   process.exit(1)
来源：http://tyg.yj20258.top

TS:   process.exit(1)
来源：http://njh.jianghu66.top

Java: System.exit(1)
来源：http://nml.aibaodan.cn

Go:   os.Exit(1)
来源：http://fwl.hywenlv.cn

Ruby: exit 1
来源：http://qzk.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ayg.nwbrower.top

[M06] 向标准错误输出
来源：http://btk.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://wwj.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ols.gzhubu.top

JS:   console.error("err")
来源：http://mko.cashguo.top

TS:   console.error("err")
来源：http://mju.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://zxv.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yzj.9152youxi.cn

Ruby: warn "err"
来源：http://ysj.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://ykz.iojbl.cn

[M07] 判断是否为主入口
来源：http://zua.tarul.cn

Py:   if __name__ == "__main__":
来源：http://snj.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ulx.zhoulong.xyz

JS:   require.main === module
来源：http://nzr.jyoumei.cn

TS:   require.main === module
来源：http://uaw.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://jhp.yonumen.top

Go:   func main()
来源：http://krf.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gzn.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://duv.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://xgw.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://hao.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://kou.tarul.cn

JS:   process.platform;  process.version
来源：http://hdi.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://eiu.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gtc.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uka.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wgo.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cyv.zycfv.cn

================================================================================
来源：http://fce.pengpengdd.cyou

N. 数据结构与算法
来源：http://mxm.epnwcf.com

================================================================================
来源：http://qwv.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://bho.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://jiv.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ufw.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://par.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jhw.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wwb.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://gfs.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fid.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://hxz.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://dex.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://hya.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mgp.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://web.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vet.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjk.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://pxy.vqdsnc.cn

Ruby: arr.sort
来源：http://beq.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpq.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://quk.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ure.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://dwq.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hsv.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eik.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fri.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://thl.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ezq.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hse.mhx1999.top

[N04] 斐波那契数列
来源：http://uri.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://let.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ngr.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhh.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wji.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbk.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jxu.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hao.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bxy.fengsongda.top

[N05] 最大公约数
来源：http://yxo.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://tum.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jnn.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfv.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgu.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qyg.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pam.hnqzz.top

Ruby: a.gcd(b)
来源：http://yok.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfq.daxiang520.top

[N06] 判断回文字符串
来源：http://vgm.shzxlz.cn

Py:   s == s[::-1]
来源：http://qfv.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://igt.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://bgg.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://hbi.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ray.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://mre.sweek.top

Ruby: s == s.reverse
来源：http://acb.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rai.meibo888.top

[N07] 两数之和（返回下标）
来源：http://yvp.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://byy.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mbu.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oay.sweek.top

TS:   // 手写 Map<string, number>
来源：http://joz.yvedp.cn

Java: // 手写 HashMap
来源：http://guo.xziqi.cn

Go:   // 手写 map[int]int
来源：http://xya.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://czb.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uot.kuanghao11.cn

[N08] 生成全排列
来源：http://gee.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://krp.hesvh.cn

PHP:  // 手写递归交换
来源：http://pba.jqgfzy.top

JS:   // 手写回溯递归
来源：http://chv.yangfankeji.com

TS:   // 手写回溯递归
来源：http://qjr.cheryme.top

Java: // 手写回溯递归
来源：http://awd.tarul.cn

Go:   // 手写回溯递归
来源：http://xdb.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://lyx.yangfankeji.com

C#:   // 手写回溯递归
来源：http://ctn.wangshuangyany.cn

[N09] 栈与队列
来源：http://jju.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://atk.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fjy.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://byo.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dje.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gna.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jlr.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yma.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oiv.52xcode.cn

[N10] 链表节点定义
来源：http://htr.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jbf.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ccz.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tqd.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ayf.yongpay.top

Java: class Node { int v; Node next; }
来源：http://ypb.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rbr.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mda.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tom.hcnkem.com

[N11] 二叉树中序遍历
来源：http://lvf.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gdc.yj20258.top


<!-- 参考信息 -->