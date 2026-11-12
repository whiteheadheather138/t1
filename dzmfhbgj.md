代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ssg.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvh.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpj.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iim.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ewq.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vwp.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qcr.fktsv.cn

[K05] 深拷贝对象
来源：http://bav.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://wek.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://uif.svipenyu.cn

JS:   structuredClone(obj)
来源：http://rjc.yuxming.cn

TS:   structuredClone(obj)
来源：http://sor.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jer.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fkm.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsu.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://soe.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://pzc.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dky.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cpo.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://snh.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fhx.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vow.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://acr.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvx.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dln.tanke756.top

[K07] 进制转换
来源：http://zkp.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hip.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ctr.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzs.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ftt.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vna.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bdw.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://run.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hvl.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://zed.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://ohg.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://lfw.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://ung.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://uol.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://feo.yanxiufei.cn

Go:   encoding/gob
来源：http://pjj.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://pjh.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wcn.bjfxy.top

================================================================================
来源：http://nvg.hfpthk.cn

L. 网络请求
来源：http://pox.jinghuilouyu.cn

================================================================================
来源：http://kie.mhx1999.top

[L01] 发送 GET 请求
来源：http://xnu.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xid.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kki.xuanzx.com

JS:   await fetch(url)
来源：http://ocd.chenzaomai.com

TS:   await fetch(url)
来源：http://bpg.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbu.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ulg.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hfv.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://elp.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://gzv.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://tdk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aiy.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gws.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yup.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://prm.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jxr.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rgm.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xnk.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://nlx.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fhk.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sqj.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iyb.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://huq.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gne.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xce.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zoz.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wzm.jinqigfzy.top

[L04] 设置超时
来源：http://lrd.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://rtk.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xai.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eew.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ouv.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibr.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqz.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jmp.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jhv.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://omf.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rfj.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dwh.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mny.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nbb.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wxh.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dpg.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yal.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://awm.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://qia.redwolf501.top

Py:   resp.json()
来源：http://hiz.hesvh.cn

PHP:  json_decode($body, true);
来源：http://fwa.yueranfly.top

JS:   await resp.json()
来源：http://ure.sysykeji.top

TS:   await resp.json()
来源：http://bsc.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tjs.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xct.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://ebc.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zhq.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://hag.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tqd.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jug.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://tyv.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://owq.dianchejie.cn

Java: resp.statusCode()
来源：http://keg.meibo888.top

Go:   resp.StatusCode
来源：http://koh.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://ueg.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://zte.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://wpf.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://khp.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://dfv.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfo.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxk.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dzg.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uov.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xmg.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jug.wangdashe.top

================================================================================
来源：http://xmh.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://frp.guowangkeji.top

================================================================================
来源：http://yln.hysaishi.cn

[M01] 读取命令行参数
来源：http://xxz.9152youxi.cn

Py:   sys.argv[1:]
来源：http://eoq.sxryk.cn

PHP:  $argv;  $argc;
来源：http://kbr.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://iqq.yonumen.top

TS:   process.argv.slice(2)
来源：http://fyc.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://wyw.pycfn.com

Go:   os.Args[1:]
来源：http://nkw.havefunace.top

Ruby: ARGV
来源：http://puk.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://qya.tianlin.xyz

[M02] 读取环境变量
来源：http://yyu.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://gaa.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lbi.fehbvm.com

JS:   process.env.HOME
来源：http://oll.xylfe.cn

TS:   process.env.HOME
来源：http://mya.316326.xyz

Java: System.getenv("HOME")
来源：http://cbu.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ass.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://ztt.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nuj.sxryk.cn

[M03] 执行外部命令
来源：http://nqd.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpd.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hoa.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pum.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kzp.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hth.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://wza.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tuw.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://gaj.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://ygb.jiagoushi.top

Py:   os.getcwd()
来源：http://yrr.yongpay.top

PHP:  getcwd();
来源：http://zrc.ybcxt.top

JS:   process.cwd()
来源：http://pho.feifeiyinyue.top

TS:   process.cwd()
来源：http://hzu.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://tjj.jinqigufen.top

Go:   os.Getwd()
来源：http://hec.bjfxy.top

Ruby: Dir.pwd
来源：http://ljt.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://kav.daria6918.cn

[M05] 设置退出码
来源：http://ona.xinyue.icu

Py:   sys.exit(1)
来源：http://feh.smart0.xyz

PHP:  exit(1);
来源：http://ocs.shuidangran.top

JS:   process.exit(1)
来源：http://gfb.ydzc1.top

TS:   process.exit(1)
来源：http://xps.daxiang520.top

Java: System.exit(1)
来源：http://uup.yuanzhike.top

Go:   os.Exit(1)
来源：http://ifk.fanxiaobao.xyz

Ruby: exit 1
来源：http://loc.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jfr.c1oappe.top

[M06] 向标准错误输出
来源：http://pwl.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://rij.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://elj.guowangkeji.top

JS:   console.error("err")
来源：http://ihd.jinghuilouyu.cn

TS:   console.error("err")
来源：http://sic.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://ibp.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hey.tianlin.xyz

Ruby: warn "err"
来源：http://nsz.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://pnr.daxiang520.top

[M07] 判断是否为主入口
来源：http://xet.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://aid.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thg.hnxiangtu.top

JS:   require.main === module
来源：http://com.xylfe.cn

TS:   require.main === module
来源：http://xpm.yonumen.top

Java: public static void main(String[] args)
来源：http://ohy.chenjidiqi.icu

Go:   func main()
来源：http://axd.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fdj.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://bpf.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://ygl.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://xgv.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://ukv.redwolf501.top

JS:   process.platform;  process.version
来源：http://kfk.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://mig.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://znd.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tdc.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pyy.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ept.uphjek.com

================================================================================
来源：http://mlh.guannengcc.top

N. 数据结构与算法
来源：http://myn.xziqi.cn

================================================================================
来源：http://pix.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://ies.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://ozg.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bvm.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmc.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfn.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mvf.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://cpo.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tfq.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dwa.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://day.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://yqy.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bgn.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://svb.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zlq.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tgg.hnqzz.top

Go:   slices.Sort(arr)
来源：http://gkr.feifeiyinyue.top

Ruby: arr.sort
来源：http://xsr.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vlu.cashguo.top

[N03] 快速排序（分治示例）
来源：http://rlz.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lut.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://rqk.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ylg.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dca.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yit.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ovb.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ecn.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://lxq.mhx1999.top

[N04] 斐波那契数列
来源：http://fmf.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uzh.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://adn.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fth.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yrn.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uju.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://llk.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tuw.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qii.aizwys.cn

[N05] 最大公约数
来源：http://lci.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://vch.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://knv.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cun.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awr.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kcx.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpn.cashguo.top

Ruby: a.gcd(b)
来源：http://nvs.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tsh.hnxiangtu.top

[N06] 判断回文字符串
来源：http://cqb.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://wts.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://sra.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://gtj.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://imv.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://duz.iojbl.cn

Go:   // 双指针从两端比较
来源：http://zww.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://pzi.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sup.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://chz.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dnh.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jtr.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rvo.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://ajf.yueranfly.top

Java: // 手写 HashMap
来源：http://ltt.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://jim.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://ffv.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://jqz.xuanzx.com

[N08] 生成全排列
来源：http://yqb.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://gmx.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://nev.yfazqb.com

JS:   // 手写回溯递归
来源：http://tte.iojbl.cn

TS:   // 手写回溯递归
来源：http://gpg.nanxuanxn.top

Java: // 手写回溯递归
来源：http://sfd.shzxlz.cn

Go:   // 手写回溯递归
来源：http://dsw.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://eas.zdqjudy.top

C#:   // 手写回溯递归
来源：http://yaa.sxryk.cn

[N09] 栈与队列
来源：http://dbr.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uwq.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gqb.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jbh.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jch.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ttp.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xbk.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oto.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oay.bbcook.cn

[N10] 链表节点定义
来源：http://sze.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vbl.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://xnl.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ohw.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dix.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://qeo.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://igg.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bsw.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://way.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://bir.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nxg.daria6918.cn

PHP:  // 手写递归函数
来源：http://fae.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gko.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jnx.fzhhl.top

Java: // 手写递归
来源：http://hqz.ydzc1.top

Go:   // 手写递归
来源：http://lxo.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mfh.yj202588.top

C#:   // 手写递归
来源：http://jub.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jgj.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://shl.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ayk.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tml.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yag.fanxiaobao.xyz


<!-- 参考信息 -->