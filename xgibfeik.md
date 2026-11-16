代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jtz.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdr.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxe.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gsh.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqa.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vbl.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://noi.jqgufenzy.top

[K05] 深拷贝对象
来源：http://pzf.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://tdu.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://oxp.0kj1m.cn

JS:   structuredClone(obj)
来源：http://nzv.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://mcm.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xfv.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tjw.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mkq.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ftu.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://ndd.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ilk.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zyw.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aor.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://umq.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://haq.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gtt.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ihl.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://inx.xuetiantiany.cn

[K07] 进制转换
来源：http://tnq.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kny.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://urb.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oij.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ujm.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dcd.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vkz.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hxi.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rmh.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://gpn.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://yvn.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qax.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mec.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://tjp.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hkm.pycfn.com

Go:   encoding/gob
来源：http://oco.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://rdx.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ydc.feifeiyinyue.top

================================================================================
来源：http://epa.zhiwuduotai.top

L. 网络请求
来源：http://mht.quarkkingdee.top

================================================================================
来源：http://jor.sxryk.cn

[L01] 发送 GET 请求
来源：http://sas.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xhi.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jve.cqqwz.cn

JS:   await fetch(url)
来源：http://gox.sysykeji.top

TS:   await fetch(url)
来源：http://wwi.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wlj.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://lko.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kml.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgq.xylfe.cn

[L02] 发送 POST JSON
来源：http://cms.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dbq.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iso.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bra.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tan.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fqy.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ngp.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sdo.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cmc.gotoacloud.top

[L03] 设置自定义请求头
来源：http://ptn.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bpd.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wgw.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mih.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://euw.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mwo.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hhj.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qjs.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ijk.yvedp.cn

[L04] 设置超时
来源：http://ghh.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://ssw.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ncy.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ocr.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ecv.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jtd.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ejz.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zkh.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://elq.52xcode.cn

[L05] 上传文件（multipart）
来源：http://iwv.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nat.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wub.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uhr.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tqe.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vdf.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aou.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dua.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uvf.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ixu.hongshengwenyu.top

Py:   resp.json()
来源：http://keu.iojbl.cn

PHP:  json_decode($body, true);
来源：http://vuq.svipenyu.cn

JS:   await resp.json()
来源：http://ipd.jinqigfzy.top

TS:   await resp.json()
来源：http://vvi.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gbr.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hks.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://spo.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ffp.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://saf.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lin.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zea.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://pij.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://eay.ydzc1.top

Java: resp.statusCode()
来源：http://gje.uphjek.com

Go:   resp.StatusCode
来源：http://ayr.fehbvm.com

Ruby: resp.code.to_i
来源：http://uou.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://nhl.guannengcc.top

[L08] 并发请求多个地址
来源：http://hue.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wca.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://qsv.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imv.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzt.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gqz.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpa.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ysp.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://epq.vqdsnc.cn

================================================================================
来源：http://rom.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://tmi.chenzaomai.com

================================================================================
来源：http://xsd.nanxinkj.top

[M01] 读取命令行参数
来源：http://rjl.redwolf501.top

Py:   sys.argv[1:]
来源：http://sos.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://lmz.meibo888.top

JS:   process.argv.slice(2)
来源：http://pdy.guannengcc.top

TS:   process.argv.slice(2)
来源：http://bpj.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://amt.jqgufenzy.top

Go:   os.Args[1:]
来源：http://cdb.yj20258888.top

Ruby: ARGV
来源：http://byy.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://kvo.feifeiyinyue.top

[M02] 读取环境变量
来源：http://ndz.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://mlr.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cjl.cheryme.top

JS:   process.env.HOME
来源：http://xgj.yongpay.top

TS:   process.env.HOME
来源：http://sun.yfazqb.com

Java: System.getenv("HOME")
来源：http://ugd.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxp.meibo888.top

Ruby: ENV["HOME"]
来源：http://yut.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ihz.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://vkw.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mfn.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oem.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mdj.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qdm.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zvy.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://idp.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://jkc.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://lca.hcnkem.com

[M04] 获取当前工作目录
来源：http://wsr.hcnkem.com

Py:   os.getcwd()
来源：http://squ.sxryk.cn

PHP:  getcwd();
来源：http://kqe.hnqzz.top

JS:   process.cwd()
来源：http://xrm.chenzaomai.com

TS:   process.cwd()
来源：http://bxt.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://eri.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://mac.zdqjudy.top

Ruby: Dir.pwd
来源：http://ssu.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qhy.redwolf501.top

[M05] 设置退出码
来源：http://tmn.chenzaomai.com

Py:   sys.exit(1)
来源：http://vij.zhiwuduotai.top

PHP:  exit(1);
来源：http://rty.tanke756.top

JS:   process.exit(1)
来源：http://mhr.0kj1m.cn

TS:   process.exit(1)
来源：http://alo.cdnleiting.top

Java: System.exit(1)
来源：http://mxf.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://obp.zhengqikj.top

Ruby: exit 1
来源：http://ohn.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ytg.hesvh.cn

[M06] 向标准错误输出
来源：http://hid.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://hln.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oqa.fanxiaobao.xyz

JS:   console.error("err")
来源：http://skj.uphjek.com

TS:   console.error("err")
来源：http://ixy.zycfv.cn

Java: System.err.println("err")
来源：http://hcy.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nbl.epnwcf.com

Ruby: warn "err"
来源：http://gxl.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://psq.shzxlz.cn

[M07] 判断是否为主入口
来源：http://aoe.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://vrz.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zjt.tarul.cn

JS:   require.main === module
来源：http://tel.ctjpmb.com

TS:   require.main === module
来源：http://dld.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://eci.birdmap.top

Go:   func main()
来源：http://dhn.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nrx.bjfxy.top

C#:   static void Main(string[] args)
来源：http://ueu.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://tvi.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://xbh.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://lmg.guannengcc.top

JS:   process.platform;  process.version
来源：http://nri.vehdjk.com

TS:   process.platform;  process.version
来源：http://zin.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eil.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://myq.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvn.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://kyo.xuetiantiany.cn

================================================================================
来源：http://lzd.jinqigufen.top

N. 数据结构与算法
来源：http://qjt.tanke756.top

================================================================================
来源：http://mrr.cheryme.top

[N01] 二分查找（有序数组）
来源：http://qpa.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hhf.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dky.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fsp.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kxs.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fqe.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://asl.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wav.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tqk.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://tni.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://dtm.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ppd.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ezf.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbj.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfk.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://fft.yj20258888.top

Ruby: arr.sort
来源：http://xms.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://arl.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://jko.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://but.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://tcf.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zpv.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wrf.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ebs.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lba.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ges.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zel.dianchejie.cn

[N04] 斐波那契数列
来源：http://kib.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rdm.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iph.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mte.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpe.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zpk.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nxi.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vqi.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eiz.andypj.xyz

[N05] 最大公约数
来源：http://zaq.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://bkg.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nwd.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fln.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lrg.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qxz.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xzr.hywenlv.cn

Ruby: a.gcd(b)
来源：http://xif.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cfn.aizwys.cn

[N06] 判断回文字符串
来源：http://eak.shzxlz.cn

Py:   s == s[::-1]
来源：http://ytd.fzhhl.top

PHP:  $s === strrev($s);
来源：http://ppx.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://kwc.gogol.net.cn

TS:   s === [...s].reverse().join("")
来源：http://agr.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xys.sysykeji.top

Go:   // 双指针从两端比较
来源：http://cir.svipenyu.cn

Ruby: s == s.reverse
来源：http://fqe.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dzw.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://xnb.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ixm.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qtt.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://naw.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://ilm.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://prt.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://iks.guowangkeji.top

Ruby: // 手写 Hash
来源：http://xuw.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gjo.52xcode.cn

[N08] 生成全排列
来源：http://hho.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://dkb.nanxinkj.top

PHP:  // 手写递归交换
来源：http://pap.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://vlg.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://ysb.shzxlz.cn

Java: // 手写回溯递归
来源：http://kkv.sysykeji.top

Go:   // 手写回溯递归
来源：http://lrq.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://lky.yj20258888.top

C#:   // 手写回溯递归
来源：http://msi.feifeiyinyue.top

[N09] 栈与队列
来源：http://ifi.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oss.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gtk.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qdi.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kic.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jpb.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sja.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fto.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://umq.uphjek.com

[N10] 链表节点定义
来源：http://zwl.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fgn.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vic.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gpy.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kgi.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://jpq.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://noa.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wew.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fbc.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://yxo.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kzg.yangfankeji.com

PHP:  // 手写递归函数
来源：http://ozg.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dzw.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://env.jlsjyb.cn

Java: // 手写递归
来源：http://znw.chenlongwang.top

Go:   // 手写递归
来源：http://bjx.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qqn.yonumen.top

C#:   // 手写递归
来源：http://aqq.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://did.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://icq.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://foc.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mzu.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ypt.yongpay.top


<!-- 参考信息 -->