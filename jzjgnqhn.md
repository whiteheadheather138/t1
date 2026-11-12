代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://uno.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gkb.bjfxy.top

[K04] 读取 JSON 文件
来源：http://tqz.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vwx.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://duh.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpq.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uns.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jdm.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ryn.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xbp.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sxg.52xcode.cn

[K05] 深拷贝对象
来源：http://ufi.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://wqj.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://xmg.ctjpmb.com

JS:   structuredClone(obj)
来源：http://byy.epnwcf.com

TS:   structuredClone(obj)
来源：http://eqa.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wgh.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://szi.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://now.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sww.guannengcc.top

[K06] 解析 URL 查询串
来源：http://fxd.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qty.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qfl.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zyv.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yaf.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vzl.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pfa.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lxz.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pxw.aizwys.cn

[K07] 进制转换
来源：http://lzb.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qva.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sxs.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fru.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kyz.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aax.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://piu.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ctq.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://glp.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://ipf.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://olq.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sfk.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://rwt.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://hto.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rlf.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://bfd.sweek.top

Ruby: Marshal.dump(obj)
来源：http://fht.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://osk.fzhhl.top

================================================================================
来源：http://nfx.shangyingyoupin.top

L. 网络请求
来源：http://pdu.shzxlz.cn

================================================================================
来源：http://sld.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://rar.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hit.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://beg.xylfe.cn

JS:   await fetch(url)
来源：http://ala.redwolf501.top

TS:   await fetch(url)
来源：http://dee.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kin.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://dyq.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://qjc.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ukp.yonumen.top

[L02] 发送 POST JSON
来源：http://mkj.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://igs.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ysr.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdr.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmo.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jsp.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zuq.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dsi.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://btv.yj202588.top

[L03] 设置自定义请求头
来源：http://vag.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://can.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lrs.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://knq.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvk.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rdb.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://szd.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://epf.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zwy.jlsjyb.cn

[L04] 设置超时
来源：http://hcl.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://rla.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jot.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkj.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofg.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dia.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wey.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kts.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jnq.bbcook.cn

[L05] 上传文件（multipart）
来源：http://ndk.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hih.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqg.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wkp.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jiq.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pgy.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bxo.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://opq.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nic.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://gjt.guannengcc.top

Py:   resp.json()
来源：http://gdf.aizwys.cn

PHP:  json_decode($body, true);
来源：http://dzs.ehwqpu.com

JS:   await resp.json()
来源：http://qwy.nwbrower.top

TS:   await resp.json()
来源：http://wfk.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kwu.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qpi.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://cel.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qki.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://dio.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gmk.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zkf.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://mtu.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://rwm.uphjek.com

Java: resp.statusCode()
来源：http://jkz.daxiang520.top

Go:   resp.StatusCode
来源：http://lbt.yangfankeji.com

Ruby: resp.code.to_i
来源：http://mpf.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://cvu.hywenlv.cn

[L08] 并发请求多个地址
来源：http://lyd.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://acz.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://hqc.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crr.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhc.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://czx.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnv.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fuu.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nnf.nanxinkj.top

================================================================================
来源：http://rxt.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://cvs.nanxuanxn.top

================================================================================
来源：http://jxm.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://qlr.ppjwa.cn

Py:   sys.argv[1:]
来源：http://gnu.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://abj.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://ybs.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://ufo.ivvv.top

Java: args 数组（main 方法参数）
来源：http://afm.nanxinkj.top

Go:   os.Args[1:]
来源：http://sth.zhixingplan.top

Ruby: ARGV
来源：http://oam.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://jxg.ctjpmb.com

[M02] 读取环境变量
来源：http://dlv.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://qvl.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sue.tarul.cn

JS:   process.env.HOME
来源：http://twd.yangfankeji.com

TS:   process.env.HOME
来源：http://mqn.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://zpm.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rmb.zycfv.cn

Ruby: ENV["HOME"]
来源：http://mzv.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://skp.gaohongyu789.top

[M03] 执行外部命令
来源：http://ntn.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rgr.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hss.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ast.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nvg.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xkj.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://xih.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://fbh.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://pva.tanke756.top

[M04] 获取当前工作目录
来源：http://iks.xinyue.icu

Py:   os.getcwd()
来源：http://pbn.zhoulong.xyz

PHP:  getcwd();
来源：http://bdk.cdnleiting.top

JS:   process.cwd()
来源：http://ekt.snrcjt.cn

TS:   process.cwd()
来源：http://ueo.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://scv.pengpengdd.cyou

Go:   os.Getwd()
来源：http://kec.xylfe.cn

Ruby: Dir.pwd
来源：http://gyd.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dfc.smart0.xyz

[M05] 设置退出码
来源：http://sng.birdmap.top

Py:   sys.exit(1)
来源：http://mma.fengsongda.top

PHP:  exit(1);
来源：http://pgk.fzhhl.top

JS:   process.exit(1)
来源：http://vyb.shangyingyoupin.top

TS:   process.exit(1)
来源：http://cyx.pengpengdd.cyou

Java: System.exit(1)
来源：http://rcb.hcnkem.com

Go:   os.Exit(1)
来源：http://dzk.tarul.cn

Ruby: exit 1
来源：http://sni.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tff.daxiang520.top

[M06] 向标准错误输出
来源：http://yhn.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://uwo.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oeq.316326.xyz

JS:   console.error("err")
来源：http://slw.zhongyouzk.top

TS:   console.error("err")
来源：http://uju.ybcxt.top

Java: System.err.println("err")
来源：http://sut.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jyb.yuxming.cn

Ruby: warn "err"
来源：http://sop.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://yku.hcnkem.com

[M07] 判断是否为主入口
来源：http://vps.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://isq.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pjz.yonumen.top

JS:   require.main === module
来源：http://axl.yfazqb.com

TS:   require.main === module
来源：http://qoi.52xcode.cn

Java: public static void main(String[] args)
来源：http://anv.fehbvm.com

Go:   func main()
来源：http://hex.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eff.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://hto.tarul.cn

[M08] 获取系统与运行时信息
来源：http://clh.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://npu.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://sba.yongpay.top

JS:   process.platform;  process.version
来源：http://ehe.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://drl.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qgj.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqy.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://znl.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qdc.shzxlz.cn

================================================================================
来源：http://lta.nanxinkj.top

N. 数据结构与算法
来源：http://ypq.bbcook.cn

================================================================================
来源：http://zlh.tanke756.top

[N01] 二分查找（有序数组）
来源：http://izq.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://kfa.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ezl.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fyk.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbi.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://dye.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://sps.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zcn.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://bgm.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://wbl.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://wfg.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aws.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pxy.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxd.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emi.52xcode.cn

Go:   slices.Sort(arr)
来源：http://dcy.redwolf501.top

Ruby: arr.sort
来源：http://bfy.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hkq.cashguo.top

[N03] 快速排序（分治示例）
来源：http://ygq.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://afz.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://qoo.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qbe.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofg.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kts.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ljl.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://onn.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://fst.shuidangran.top

[N04] 斐波那契数列
来源：http://zhd.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://psi.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oqm.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzu.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibv.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vsf.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ydb.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bks.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wqb.nanxuanxn.top

[N05] 最大公约数
来源：http://edc.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://cfy.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dsj.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhy.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwm.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://shz.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rgj.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://szd.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://avr.chenzaomai.com

[N06] 判断回文字符串
来源：http://izq.zhoulong.xyz

Py:   s == s[::-1]
来源：http://owl.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://otk.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://rps.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://dpl.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://upu.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://qhn.xylfe.cn

Ruby: s == s.reverse
来源：http://cno.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://qnu.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://eqc.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ysl.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tlm.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://ueb.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://cdc.vqdsnc.cn

Java: // 手写 HashMap
来源：http://moe.fzhhl.top

Go:   // 手写 map[int]int
来源：http://jku.gzhubu.top

Ruby: // 手写 Hash
来源：http://xaw.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://vbx.cqqwz.cn

[N08] 生成全排列
来源：http://ksy.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://pbp.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://ges.smart0.xyz

JS:   // 手写回溯递归
来源：http://wze.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://mal.hysaishi.cn

Java: // 手写回溯递归
来源：http://edn.xziqi.cn

Go:   // 手写回溯递归
来源：http://igp.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://lpn.birdmap.top

C#:   // 手写回溯递归
来源：http://mgz.wangdashe.top

[N09] 栈与队列
来源：http://zpx.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://njn.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mwi.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sjt.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yuu.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yqe.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vzm.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cqd.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ray.tian-w.cn

[N10] 链表节点定义
来源：http://vub.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lpz.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://aez.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wyd.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bgi.havefunace.top

Java: class Node { int v; Node next; }
来源：http://jvn.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://yzh.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://ggq.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ztu.wangdashe.top

[N11] 二叉树中序遍历
来源：http://rgy.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xgg.zycfv.cn

PHP:  // 手写递归函数
来源：http://uom.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdl.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxx.vqdsnc.cn

Java: // 手写递归
来源：http://pxy.xziqi.cn

Go:   // 手写递归
来源：http://sfc.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zlr.9152youxi.cn

C#:   // 手写递归
来源：http://mjs.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zqf.wangshuangyany.cn


<!-- 参考信息 -->