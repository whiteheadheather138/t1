代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://tvd.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://elq.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://zxx.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yoh.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ski.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://noa.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ung.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kah.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://upr.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://max.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zfa.52xcode.cn

[K05] 深拷贝对象
来源：http://hyw.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://ktn.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://nem.hcnkem.com

JS:   structuredClone(obj)
来源：http://ebl.zhengqikj.top

TS:   structuredClone(obj)
来源：http://qrc.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mzf.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://efb.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cqk.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fuk.redwolf501.top

[K06] 解析 URL 查询串
来源：http://qoa.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://szz.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fdt.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rsm.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qds.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tmh.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pub.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tws.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cmz.cashguo.top

[K07] 进制转换
来源：http://tub.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aob.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xsp.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kju.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://avn.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jml.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nxn.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsj.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pyj.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://btg.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://lbe.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aam.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://xob.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://eaj.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kyv.zdqjudy.top

Go:   encoding/gob
来源：http://rfn.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://sxi.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wbr.iojbl.cn

================================================================================
来源：http://wae.fehbvm.com

L. 网络请求
来源：http://pac.zhixingplan.top

================================================================================
来源：http://pdm.tanke756.top

[L01] 发送 GET 请求
来源：http://ztj.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tth.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tdo.cqqwz.cn

JS:   await fetch(url)
来源：http://gah.kuanghao11.cn

TS:   await fetch(url)
来源：http://llz.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tcr.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://bui.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://adj.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tcr.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://fcs.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://kky.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wkc.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bsd.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovz.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aes.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wcz.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gpd.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ilk.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://ohi.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iyc.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bis.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://awm.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irw.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kft.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ufz.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xpp.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gbp.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://nnw.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://fjh.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://emu.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zng.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rdj.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wsu.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vxg.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bpt.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://esg.zycfv.cn

[L05] 上传文件（multipart）
来源：http://yyy.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zys.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qex.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qyw.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vlu.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbb.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ztp.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vpw.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kod.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://ecl.havefunace.top

Py:   resp.json()
来源：http://ilu.cucudq.cn

PHP:  json_decode($body, true);
来源：http://bhe.dashuyun.cn

JS:   await resp.json()
来源：http://dob.cqqwz.cn

TS:   await resp.json()
来源：http://fxr.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rvj.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vnn.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://hgu.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bgc.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://xat.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iha.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://hwm.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://sfj.52xcode.cn

Java: resp.statusCode()
来源：http://jaa.tarul.cn

Go:   resp.StatusCode
来源：http://uhr.316326.xyz

Ruby: resp.code.to_i
来源：http://szw.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://nvo.wangdashe.top

[L08] 并发请求多个地址
来源：http://pve.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wgp.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://lnk.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilt.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gww.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dim.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vyi.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://htm.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://raa.yuanzhike.top

================================================================================
来源：http://msf.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://wyb.tian-w.cn

================================================================================
来源：http://whu.shuidangran.top

[M01] 读取命令行参数
来源：http://sgc.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://peb.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://lgk.xylfe.cn

JS:   process.argv.slice(2)
来源：http://mvm.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://yuq.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://bmw.jqgfzy.top

Go:   os.Args[1:]
来源：http://fkj.ydjk.org.cn

Ruby: ARGV
来源：http://urb.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://doj.jqgufenzy.top

[M02] 读取环境变量
来源：http://ylb.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://lqm.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xuu.c1oappe.top

JS:   process.env.HOME
来源：http://ddp.aibaodan.cn

TS:   process.env.HOME
来源：http://glw.c1oappe.top

Java: System.getenv("HOME")
来源：http://auo.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uel.bjfxy.top

Ruby: ENV["HOME"]
来源：http://udi.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hao.chenlongwang.top

[M03] 执行外部命令
来源：http://lnp.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rfi.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxx.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ayb.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://ylr.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gqm.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://edl.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://wno.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://fpj.dianchejie.cn

[M04] 获取当前工作目录
来源：http://kzl.uphjek.com

Py:   os.getcwd()
来源：http://tmj.meibo888.top

PHP:  getcwd();
来源：http://oau.fengsongda.top

JS:   process.cwd()
来源：http://ibn.bbcook.cn

TS:   process.cwd()
来源：http://lzv.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://kdr.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://rwq.hywenlv.cn

Ruby: Dir.pwd
来源：http://yee.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://huf.tian-w.cn

[M05] 设置退出码
来源：http://alk.xinyue.icu

Py:   sys.exit(1)
来源：http://olb.cashguo.top

PHP:  exit(1);
来源：http://gcg.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://ifa.tianlin.xyz

TS:   process.exit(1)
来源：http://gso.fktsv.cn

Java: System.exit(1)
来源：http://syf.xziqi.cn

Go:   os.Exit(1)
来源：http://xxf.yonumen.top

Ruby: exit 1
来源：http://kpm.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://die.xziqi.cn

[M06] 向标准错误输出
来源：http://bpi.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://edc.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://uxh.wangdashe.top

JS:   console.error("err")
来源：http://xbv.zhixingplan.top

TS:   console.error("err")
来源：http://usk.jinqigufen.top

Java: System.err.println("err")
来源：http://gbp.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ihr.cucudq.cn

Ruby: warn "err"
来源：http://dro.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://fal.zdqjudy.top

[M07] 判断是否为主入口
来源：http://xku.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://fcx.vqdsnc.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gwt.cashguo.top

JS:   require.main === module
来源：http://usb.zhaomingkeji.xyz

TS:   require.main === module
来源：http://ccx.cdnleiting.top

Java: public static void main(String[] args)
来源：http://xyh.snrcjt.cn

Go:   func main()
来源：http://ytt.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zld.hesvh.cn

C#:   static void Main(string[] args)
来源：http://fbn.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://aju.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://rli.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://iks.aibaodan.cn

JS:   process.platform;  process.version
来源：http://qwm.yvedp.cn

TS:   process.platform;  process.version
来源：http://gxx.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dqe.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cng.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zoz.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vrx.ydzc1.top

================================================================================
来源：http://dwy.hfpthk.cn

N. 数据结构与算法
来源：http://giw.yangfankeji.com

================================================================================
来源：http://tou.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://rbm.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://ywq.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hxg.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tza.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcu.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://prz.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://aql.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wnr.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lhd.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://oub.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://qgg.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fkw.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://guh.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fyh.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://upa.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://pfi.yj20258.top

Ruby: arr.sort
来源：http://npl.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lii.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://ydc.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lsi.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://qge.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://apb.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kbs.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jpk.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ugk.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://agq.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yma.dashuyun.cn

[N04] 斐波那契数列
来源：http://iud.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qzh.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yca.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxh.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mql.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iir.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qif.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cwf.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://inq.fzhhl.top

[N05] 最大公约数
来源：http://rgu.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://jce.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://htf.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ihj.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qfw.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fhy.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sne.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://lxk.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfe.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://msb.0kj1m.cn

Py:   s == s[::-1]
来源：http://bgh.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://loc.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://qnf.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://hgh.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://trz.vehdjk.com

Go:   // 双指针从两端比较
来源：http://tnj.meibo888.top

Ruby: s == s.reverse
来源：http://bhc.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cyr.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://zoi.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdn.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pyf.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jmn.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://khs.jinqigufen.top

Java: // 手写 HashMap
来源：http://xbc.wangdashe.top

Go:   // 手写 map[int]int
来源：http://teu.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://kau.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://wkn.ydjk.org.cn

[N08] 生成全排列
来源：http://cgj.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://xiy.c1oappe.top

PHP:  // 手写递归交换
来源：http://ddo.wangdashe.top

JS:   // 手写回溯递归
来源：http://aci.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://xso.redwolf501.top

Java: // 手写回溯递归
来源：http://zjh.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://njl.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://blt.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://auy.yj20258888.top

[N09] 栈与队列
来源：http://wre.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uqv.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://npz.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ggd.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://haz.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://owt.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kdl.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qhx.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lmr.ivvv.top

[N10] 链表节点定义
来源：http://ncs.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mix.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ejm.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nbp.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pot.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://fgd.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://hes.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://taf.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://guj.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://rya.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nzd.sweek.top

PHP:  // 手写递归函数
来源：http://zqg.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uen.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bku.jinyuanbaomall.cn

Java: // 手写递归
来源：http://fdb.guannengcc.top

Go:   // 手写递归
来源：http://eop.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdy.xuanzx.com

C#:   // 手写递归
来源：http://lfs.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://msw.quarkkingdee.top


<!-- 参考信息 -->