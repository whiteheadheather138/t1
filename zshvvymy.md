代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://sra.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hpp.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cbj.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lfr.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kry.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ill.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://lmr.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bor.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aav.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jcr.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xbh.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ukd.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyl.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nqs.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kck.gotoacloud.top

[K05] 深拷贝对象
来源：http://xul.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://hdc.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://ryb.tian-w.cn

JS:   structuredClone(obj)
来源：http://bca.smart0.xyz

TS:   structuredClone(obj)
来源：http://duk.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qyr.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hed.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zbm.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zjt.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://vmk.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fuk.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ksn.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yap.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uyo.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxr.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ebc.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ofe.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rhk.pycfn.com

[K07] 进制转换
来源：http://pjd.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mkb.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eze.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jmg.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xww.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://isw.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjk.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hjk.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cdc.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ybn.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://jgp.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ywx.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://gkz.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://jyo.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hyi.sweek.top

Go:   encoding/gob
来源：http://vfe.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://zpw.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xbw.zycfv.cn

================================================================================
来源：http://fmv.fanxiaobao.xyz

L. 网络请求
来源：http://bpw.uphjek.com

================================================================================
来源：http://clg.yvedp.cn

[L01] 发送 GET 请求
来源：http://qfz.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eih.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hxh.svipenyu.cn

JS:   await fetch(url)
来源：http://ode.nanxuanxn.top

TS:   await fetch(url)
来源：http://qjc.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kay.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://mbh.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yxl.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qph.cashguo.top

[L02] 发送 POST JSON
来源：http://erb.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oze.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lcl.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccw.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nwy.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iyx.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://msu.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bup.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gmp.yongpay.top

[L03] 设置自定义请求头
来源：http://blb.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://muu.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gyc.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ils.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgm.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nmr.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://csq.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://niz.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pzv.cashguo.top

[L04] 设置超时
来源：http://oul.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://qyu.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sro.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ihf.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yei.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://slo.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ewq.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rzy.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wvl.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://vqw.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qea.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nsy.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bdd.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gil.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ecv.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dlb.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fip.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bff.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://xtm.dashuyun.cn

Py:   resp.json()
来源：http://qhe.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://kvh.gzhubu.top

JS:   await resp.json()
来源：http://ftf.chenjidiqi.icu

TS:   await resp.json()
来源：http://bnv.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cqx.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugp.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://yyt.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ftl.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://rff.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://maw.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wmg.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://tgp.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://nsr.yvedp.cn

Java: resp.statusCode()
来源：http://gwf.hysaishi.cn

Go:   resp.StatusCode
来源：http://pxy.cashguo.top

Ruby: resp.code.to_i
来源：http://han.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://com.xziqi.cn

[L08] 并发请求多个地址
来源：http://fly.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fkt.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://mwt.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eis.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwe.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://crh.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://swm.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wed.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://srh.xinyue.icu

================================================================================
来源：http://brl.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://rzp.pengpengdd.cyou

================================================================================
来源：http://lwr.gotoacloud.top

[M01] 读取命令行参数
来源：http://zad.tian-w.cn

Py:   sys.argv[1:]
来源：http://cmc.hcnkem.com

PHP:  $argv;  $argc;
来源：http://dvd.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://inu.smart0.xyz

TS:   process.argv.slice(2)
来源：http://qkt.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://adq.aibaodan.cn

Go:   os.Args[1:]
来源：http://ecy.hcnkem.com

Ruby: ARGV
来源：http://qpv.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://qsz.zhixingplan.top

[M02] 读取环境变量
来源：http://oip.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://gti.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dnn.pengpengdd.cyou

JS:   process.env.HOME
来源：http://knt.snrcjt.cn

TS:   process.env.HOME
来源：http://vyh.52xcode.cn

Java: System.getenv("HOME")
来源：http://grc.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bwg.xylfe.cn

Ruby: ENV["HOME"]
来源：http://fzc.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dgg.svipenyu.cn

[M03] 执行外部命令
来源：http://hgo.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wsw.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ibw.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://rcs.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://fhk.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pcd.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ajy.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nmq.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://pyg.sysykeji.top

[M04] 获取当前工作目录
来源：http://mro.zhijiandao.cn

Py:   os.getcwd()
来源：http://dld.fengsongda.top

PHP:  getcwd();
来源：http://sci.fengsongda.top

JS:   process.cwd()
来源：http://qzn.feifeiyinyue.top

TS:   process.cwd()
来源：http://npq.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://mrx.sjlbkw.cn

Go:   os.Getwd()
来源：http://cxt.epnwcf.com

Ruby: Dir.pwd
来源：http://vyw.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bpo.zhijiandao.cn

[M05] 设置退出码
来源：http://zrx.hnqzz.top

Py:   sys.exit(1)
来源：http://wvo.aibaodan.cn

PHP:  exit(1);
来源：http://wzi.sxryk.cn

JS:   process.exit(1)
来源：http://fgn.316326.xyz

TS:   process.exit(1)
来源：http://wxr.bjfxy.top

Java: System.exit(1)
来源：http://gmi.sjlbkw.cn

Go:   os.Exit(1)
来源：http://agx.uphjek.com

Ruby: exit 1
来源：http://sfn.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zlu.shanyushiyangtech.top

[M06] 向标准错误输出
来源：http://wbv.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://wjq.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ggb.haohaochexian.top

JS:   console.error("err")
来源：http://iys.tanke756.top

TS:   console.error("err")
来源：http://lcu.aibaodan.cn

Java: System.err.println("err")
来源：http://xnt.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gbd.ctjpmb.com

Ruby: warn "err"
来源：http://ozy.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://noh.yongpay.top

[M07] 判断是否为主入口
来源：http://tgv.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://gqw.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sbd.daria6918.cn

JS:   require.main === module
来源：http://zns.ywan-chungtsiang.top

TS:   require.main === module
来源：http://pmv.yj202588.top

Java: public static void main(String[] args)
来源：http://qum.yj20258888.top

Go:   func main()
来源：http://zri.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hmn.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://lnn.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://bcp.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://qxv.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://iwi.redwolf501.top

JS:   process.platform;  process.version
来源：http://clc.hammf.cn

TS:   process.platform;  process.version
来源：http://cin.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hff.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rap.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xaq.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vap.ctjpmb.com

================================================================================
来源：http://ixu.jinghuilouyu.cn

N. 数据结构与算法
来源：http://sig.9152youxi.cn

================================================================================
来源：http://sku.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://gmz.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://shw.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bsz.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zud.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lrd.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://gfj.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://cai.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://brp.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://xzh.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://adk.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://wre.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://brs.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://efw.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bcu.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iwg.yj202588.top

Go:   slices.Sort(arr)
来源：http://nqo.jinqigfzy.top

Ruby: arr.sort
来源：http://jef.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mcx.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://cdz.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pgy.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://uwn.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcm.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxe.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qyi.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vun.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://upd.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://ssq.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://rwn.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://itr.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qvq.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jtg.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yqd.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ohl.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fai.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kex.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dbd.smart0.xyz

[N05] 最大公约数
来源：http://vvf.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://jcc.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyn.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iey.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjr.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://few.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yzf.fengsongda.top

Ruby: a.gcd(b)
来源：http://emd.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nkt.wangdashe.top

[N06] 判断回文字符串
来源：http://emo.0kj1m.cn

Py:   s == s[::-1]
来源：http://dqp.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://pzv.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://vhz.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://tlc.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nti.xylfe.cn

Go:   // 双指针从两端比较
来源：http://xcq.vehdjk.com

Ruby: s == s.reverse
来源：http://qsw.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://okz.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://ldy.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dtq.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vkl.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qdt.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://oem.hywenlv.cn

Java: // 手写 HashMap
来源：http://mlc.yfazqb.com

Go:   // 手写 map[int]int
来源：http://nsi.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://xls.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://vpo.shangyingyoupin.top

[N08] 生成全排列
来源：http://zmq.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://ahr.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://xbf.yuanzhike.top

JS:   // 手写回溯递归
来源：http://dxm.yuxming.cn

TS:   // 手写回溯递归
来源：http://dpd.sxryk.cn

Java: // 手写回溯递归
来源：http://jxq.pycfn.com

Go:   // 手写回溯递归
来源：http://nfh.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://itf.hfpthk.cn

C#:   // 手写回溯递归
来源：http://zti.tianlin.xyz

[N09] 栈与队列
来源：http://mmd.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vdd.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujf.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hqn.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ddz.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qyd.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uth.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dcp.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lao.ppjwa.cn

[N10] 链表节点定义
来源：http://rag.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bbp.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lkn.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pqu.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jnc.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://tui.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://fku.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://adz.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://nel.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://nig.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szo.ybcxt.top

PHP:  // 手写递归函数
来源：http://kdf.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cjn.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nfq.jinghuilouyu.cn

Java: // 手写递归
来源：http://vfm.dashuyun.cn


<!-- 参考信息 -->