代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://btj.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vrh.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwq.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avx.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kaa.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nkq.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://jyx.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jqv.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://prm.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yrt.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbi.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://can.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nwu.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tjh.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sii.hnxiangtu.top

[K05] 深拷贝对象
来源：http://bee.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://rbk.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://wvd.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://qor.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://fbd.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aln.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://azg.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mko.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ovq.yuxming.cn

[K06] 解析 URL 查询串
来源：http://trl.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lux.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gmo.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fwb.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqn.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fxk.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://kwf.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zli.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fjz.andypj.xyz

[K07] 进制转换
来源：http://klc.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lay.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xdl.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gnp.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mur.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hcz.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjw.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bpd.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ybq.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://xtl.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://rgz.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fux.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://ajr.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://vdx.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pwk.zycfv.cn

Go:   encoding/gob
来源：http://amd.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://rwq.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ldt.tanke756.top

================================================================================
来源：http://zgx.316326.xyz

L. 网络请求
来源：http://jrj.yanxiufei.cn

================================================================================
来源：http://ojg.mhx1999.top

[L01] 发送 GET 请求
来源：http://vkl.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqy.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://msl.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://qgs.cqqwz.cn

TS:   await fetch(url)
来源：http://bhp.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eld.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://gtp.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://syv.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kgy.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://kym.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://wxf.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kif.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khh.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zap.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hxx.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wld.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://arl.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://chc.dashuyun.cn

[L03] 设置自定义请求头
来源：http://ukq.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uxl.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rsh.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fuu.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mim.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nzj.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pyu.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uaq.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://trp.gaohongyu789.top

[L04] 设置超时
来源：http://ake.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://wqj.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rlh.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvo.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ucn.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rps.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dxt.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bls.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qrv.xylfe.cn

[L05] 上传文件（multipart）
来源：http://rko.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://imz.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tlk.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lce.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rtb.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fck.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nvm.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ary.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kve.yueranfly.top

[L06] 解析响应为 JSON
来源：http://xhv.52xcode.cn

Py:   resp.json()
来源：http://prj.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://zxo.jinqigfzy.top

JS:   await resp.json()
来源：http://ato.hnxiangtu.top

TS:   await resp.json()
来源：http://mfn.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://owm.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ecq.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://jlj.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yxp.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://tzj.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mlm.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ajf.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://lfd.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://auc.yfazqb.com

Java: resp.statusCode()
来源：http://kpb.zdbjq.cn

Go:   resp.StatusCode
来源：http://khp.tanke756.top

Ruby: resp.code.to_i
来源：http://kor.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://rzb.sufxvd.cn

[L08] 并发请求多个地址
来源：http://gsr.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hbo.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://gya.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uga.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://trr.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xlf.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gec.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uyn.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yot.chenlongwang.top

================================================================================
来源：http://lzs.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://xfk.mhx1999.top

================================================================================
来源：http://zvd.zdqjudy.top

[M01] 读取命令行参数
来源：http://gca.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://jpc.xinyue.icu

PHP:  $argv;  $argc;
来源：http://otl.sxryk.cn

JS:   process.argv.slice(2)
来源：http://fit.pycfn.com

TS:   process.argv.slice(2)
来源：http://pxx.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://xhg.fengsongda.top

Go:   os.Args[1:]
来源：http://vmj.cqqwz.cn

Ruby: ARGV
来源：http://afo.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://wuj.meibo888.top

[M02] 读取环境变量
来源：http://yms.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://tau.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://adw.nwbrower.top

JS:   process.env.HOME
来源：http://uii.guowangkeji.top

TS:   process.env.HOME
来源：http://unk.hysaishi.cn

Java: System.getenv("HOME")
来源：http://dnl.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jmz.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://ghu.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fzf.nanxuanxn.top

[M03] 执行外部命令
来源：http://ovk.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uhi.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dyr.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tiz.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://otp.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sfa.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qay.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ghd.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://zry.jyoumei.cn

[M04] 获取当前工作目录
来源：http://zip.sweek.top

Py:   os.getcwd()
来源：http://qxk.nanxinkj.top

PHP:  getcwd();
来源：http://lmx.ybcxt.top

JS:   process.cwd()
来源：http://wdz.sxryk.cn

TS:   process.cwd()
来源：http://hja.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://byg.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://tye.vehdjk.com

Ruby: Dir.pwd
来源：http://ydt.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://iac.chenzaomai.com

[M05] 设置退出码
来源：http://yki.fktsv.cn

Py:   sys.exit(1)
来源：http://xom.zhixingplan.top

PHP:  exit(1);
来源：http://odq.c1oappe.top

JS:   process.exit(1)
来源：http://tem.cashguo.top

TS:   process.exit(1)
来源：http://aoo.daria6918.cn

Java: System.exit(1)
来源：http://kjb.smart0.xyz

Go:   os.Exit(1)
来源：http://jkg.sjlbkw.cn

Ruby: exit 1
来源：http://thw.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xbr.hfpthk.cn

[M06] 向标准错误输出
来源：http://mtx.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://khc.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://btk.316326.xyz

JS:   console.error("err")
来源：http://jcj.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://xwg.52xcode.cn

Java: System.err.println("err")
来源：http://pih.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frf.fzhhl.top

Ruby: warn "err"
来源：http://qov.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://rxo.52xcode.cn

[M07] 判断是否为主入口
来源：http://ttt.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://dut.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ciq.jqgufenzy.top

JS:   require.main === module
来源：http://nct.jinyuanbaomall.cn

TS:   require.main === module
来源：http://eiu.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://yzm.zhaomingkeji.xyz

Go:   func main()
来源：http://dwd.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ite.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://qcp.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://zkf.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://ybz.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://txc.ivvv.top

JS:   process.platform;  process.version
来源：http://iob.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://zxu.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tds.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ddj.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pet.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mtl.sxryk.cn

================================================================================
来源：http://kni.uphjek.com

N. 数据结构与算法
来源：http://dmd.bbcook.cn

================================================================================
来源：http://nze.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://byl.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cdt.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://izl.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szk.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hzj.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dky.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://sfs.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xtz.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://pte.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://fug.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://pyf.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hgd.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cwx.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fwe.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coh.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://pet.yueranfly.top

Ruby: arr.sort
来源：http://ghc.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dmb.yonumen.top

[N03] 快速排序（分治示例）
来源：http://akd.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mcd.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://lbs.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgt.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ivj.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rya.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mws.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pbh.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://rsj.nwbrower.top

[N04] 斐波那契数列
来源：http://vrd.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pry.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://acs.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbp.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrl.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ach.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://muh.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbd.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://shi.sysykeji.top

[N05] 最大公约数
来源：http://vkv.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://lhz.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kxs.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jeh.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eiw.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dgk.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://krr.ivvv.top

Ruby: a.gcd(b)
来源：http://szw.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ofk.zdqjudy.top

[N06] 判断回文字符串
来源：http://wrk.birdmap.top

Py:   s == s[::-1]
来源：http://ltx.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://wiq.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://bal.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://opo.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cdc.yj20258.top

Go:   // 双指针从两端比较
来源：http://hto.nanxuanxn.top

Ruby: s == s.reverse
来源：http://ezx.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://amo.uphjek.com

[N07] 两数之和（返回下标）
来源：http://wsg.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tzc.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jin.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://sfs.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://jze.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://tbr.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://pua.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://yzy.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://crn.yfazqb.com

[N08] 生成全排列
来源：http://amo.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://nwf.fzhhl.top

PHP:  // 手写递归交换
来源：http://wpm.52xcode.cn

JS:   // 手写回溯递归
来源：http://tax.chenzaomai.com

TS:   // 手写回溯递归
来源：http://kyb.fzhhl.top

Java: // 手写回溯递归
来源：http://xai.smart0.xyz

Go:   // 手写回溯递归
来源：http://tdh.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://xkd.zdbjq.cn

C#:   // 手写回溯递归
来源：http://spj.feifeiyinyue.top

[N09] 栈与队列
来源：http://bfg.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wjg.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kqv.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tib.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ugt.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mjf.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cli.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oly.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hrs.xinyue.icu

[N10] 链表节点定义
来源：http://iff.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsm.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tve.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mrj.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apx.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://rnn.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://tpj.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://amw.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kxa.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://qgl.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gqk.gogol.net.cn

PHP:  // 手写递归函数
来源：http://oof.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dkq.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mcp.nwbrower.top

Java: // 手写递归
来源：http://yes.sysykeji.top


<!-- 参考信息 -->