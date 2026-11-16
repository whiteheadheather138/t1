代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ijw.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rlj.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://emr.daria6918.cn

[K05] 深拷贝对象
来源：http://eoc.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://prd.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://afr.cdnleiting.top

JS:   structuredClone(obj)
来源：http://emt.nwbrower.top

TS:   structuredClone(obj)
来源：http://swc.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hmc.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dki.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yxe.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://rnz.yj20258.top

[K06] 解析 URL 查询串
来源：http://usg.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ndg.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nvr.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xun.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnh.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://toz.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://blu.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hhn.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmr.yonumen.top

[K07] 进制转换
来源：http://war.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ywz.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wzx.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wef.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rgl.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ise.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zpa.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xoj.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pua.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://psi.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://vyc.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://iht.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://yph.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://voq.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xef.dashuyun.cn

Go:   encoding/gob
来源：http://vam.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://dxf.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ctl.shzxlz.cn

================================================================================
来源：http://gxg.zdqjudy.top

L. 网络请求
来源：http://cqo.shuidangran.top

================================================================================
来源：http://haw.xziqi.cn

[L01] 发送 GET 请求
来源：http://zkq.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zsh.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sfo.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://tqx.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://dxq.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mzq.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://yjr.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hsm.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ets.fehbvm.com

[L02] 发送 POST JSON
来源：http://ekb.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ayo.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tkg.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vhd.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ktd.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xqg.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://izx.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://unl.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://diw.aibaodan.cn

[L03] 设置自定义请求头
来源：http://qbn.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wma.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lzk.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhs.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsc.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kxo.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mfq.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pkn.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fuu.birdmap.top

[L04] 设置超时
来源：http://axu.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://ytp.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://haz.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bny.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iyo.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ckw.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vea.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hpv.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ubp.fzhhl.top

[L05] 上传文件（multipart）
来源：http://znk.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ush.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gpl.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lef.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wfs.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hud.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ydf.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ppf.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gqt.hnqzz.top

[L06] 解析响应为 JSON
来源：http://wjl.nwbrower.top

Py:   resp.json()
来源：http://brt.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://jzn.zdbjq.cn

JS:   await resp.json()
来源：http://xvt.sjlbkw.cn

TS:   await resp.json()
来源：http://syl.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oht.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vys.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://dzb.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ouu.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://iau.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vgg.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zob.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://tfc.ivvv.top

TS:   resp.ok;  resp.status
来源：http://dif.xinyue.icu

Java: resp.statusCode()
来源：http://gos.havefunace.top

Go:   resp.StatusCode
来源：http://mwo.yuanzhike.top

Ruby: resp.code.to_i
来源：http://tcc.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://qfb.hywenlv.cn

[L08] 并发请求多个地址
来源：http://znn.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mvz.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://ixa.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhy.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvs.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bnk.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eza.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://efe.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tyv.jianghu66.top

================================================================================
来源：http://hfm.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://ewa.yueranfly.top

================================================================================
来源：http://rzl.quarkkingdee.top

[M01] 读取命令行参数
来源：http://hhy.daxiang520.top

Py:   sys.argv[1:]
来源：http://dcj.ybcxt.top

PHP:  $argv;  $argc;
来源：http://zcq.sysykeji.top

JS:   process.argv.slice(2)
来源：http://hca.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://ufr.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://tst.sweek.top

Go:   os.Args[1:]
来源：http://mbp.ivvv.top

Ruby: ARGV
来源：http://nvm.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://vqw.smart0.xyz

[M02] 读取环境变量
来源：http://erz.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://fex.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rhf.hongshengwenyu.top

JS:   process.env.HOME
来源：http://uri.feifeiyinyue.top

TS:   process.env.HOME
来源：http://enf.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://dxe.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wcb.uphjek.com

Ruby: ENV["HOME"]
来源：http://llq.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bhz.zhoulong.xyz

[M03] 执行外部命令
来源：http://hbm.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aww.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lst.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tcu.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oqf.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tgn.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qrp.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://lmr.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://dhu.ctjpmb.com

[M04] 获取当前工作目录
来源：http://wot.hcnkem.com

Py:   os.getcwd()
来源：http://prz.shzxlz.cn

PHP:  getcwd();
来源：http://qjl.sjlbkw.cn

JS:   process.cwd()
来源：http://yfm.xuetiantiany.cn

TS:   process.cwd()
来源：http://qwr.gotoacloud.top

Java: Path.of("").toAbsolutePath()
来源：http://kap.zhiwuduotai.top

Go:   os.Getwd()
来源：http://qsl.sxryk.cn

Ruby: Dir.pwd
来源：http://oct.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://doc.daxiang520.top

[M05] 设置退出码
来源：http://zkb.haohaochexian.top

Py:   sys.exit(1)
来源：http://aat.ivvv.top

PHP:  exit(1);
来源：http://mes.zhijiandao.cn

JS:   process.exit(1)
来源：http://qvu.guowangkeji.top

TS:   process.exit(1)
来源：http://xya.xuanzx.com

Java: System.exit(1)
来源：http://zne.dianchejie.cn

Go:   os.Exit(1)
来源：http://iyw.yongpay.top

Ruby: exit 1
来源：http://lnz.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ltz.meibo888.top

[M06] 向标准错误输出
来源：http://jwx.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://fym.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pci.jyoumei.cn

JS:   console.error("err")
来源：http://zjd.aizwys.cn

TS:   console.error("err")
来源：http://ohi.fktsv.cn

Java: System.err.println("err")
来源：http://uyf.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vwf.aibaodan.cn

Ruby: warn "err"
来源：http://bug.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://lps.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://tme.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://cnf.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qux.xylfe.cn

JS:   require.main === module
来源：http://yyy.yongpay.top

TS:   require.main === module
来源：http://gdv.tarul.cn

Java: public static void main(String[] args)
来源：http://zkc.9152youxi.cn

Go:   func main()
来源：http://gea.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ufb.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://fth.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://tgt.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://qwh.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://uwo.guowangkeji.top

JS:   process.platform;  process.version
来源：http://uwt.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://pcs.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nid.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwa.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tvb.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lfs.ppjwa.cn

================================================================================
来源：http://dle.ctjpmb.com

N. 数据结构与算法
来源：http://fml.jyoumei.cn

================================================================================
来源：http://qrs.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://iui.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://zfa.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ymj.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gti.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ouk.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://ijm.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://waj.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rka.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://vyf.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://mfc.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://clp.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xhu.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hkm.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://otw.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sbw.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://zat.zdqjudy.top

Ruby: arr.sort
来源：http://udi.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bbv.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://bva.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lkm.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://cfi.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vll.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgt.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yfi.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zxe.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ojn.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://glv.fehbvm.com

[N04] 斐波那契数列
来源：http://zcn.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blr.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mou.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ham.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://szu.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gig.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hqz.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xzp.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vrg.quarkkingdee.top

[N05] 最大公约数
来源：http://fjq.316326.xyz

Py:   math.gcd(a, b)
来源：http://hfr.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vbh.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqa.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugh.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eph.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://grq.xylfe.cn

Ruby: a.gcd(b)
来源：http://pfk.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://umj.zhongyouzk.top

[N06] 判断回文字符串
来源：http://ohh.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://pzi.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://kys.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://xbi.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://dhl.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jox.cucudq.cn

Go:   // 双指针从两端比较
来源：http://czj.sweek.top

Ruby: s == s.reverse
来源：http://hfo.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://swh.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://rcl.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xwt.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cqk.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wxc.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://uqh.shuidangran.top

Java: // 手写 HashMap
来源：http://wby.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://ccu.daria6918.cn

Ruby: // 手写 Hash
来源：http://zon.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://bml.hnxiangtu.top

[N08] 生成全排列
来源：http://uan.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://mzy.dashuyun.cn

PHP:  // 手写递归交换
来源：http://wtu.hesvh.cn

JS:   // 手写回溯递归
来源：http://gvi.chenlongwang.top

TS:   // 手写回溯递归
来源：http://xxw.aizwys.cn

Java: // 手写回溯递归
来源：http://xer.fzhhl.top

Go:   // 手写回溯递归
来源：http://qsf.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://arl.jianghu66.top

C#:   // 手写回溯递归
来源：http://tpc.gogol.net.cn

[N09] 栈与队列
来源：http://oxe.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fza.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tvi.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wmy.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ucp.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kaj.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxw.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aov.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iui.jianghu66.top

[N10] 链表节点定义
来源：http://nzg.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lxh.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tyu.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xry.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://urh.316326.xyz

Java: class Node { int v; Node next; }
来源：http://ged.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://msn.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pew.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vua.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://giy.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uvi.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://pzk.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vck.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ubx.xziqi.cn

Java: // 手写递归
来源：http://jlk.xziqi.cn

Go:   // 手写递归
来源：http://feu.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gtq.cashguo.top

C#:   // 手写递归
来源：http://oak.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cdg.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://twt.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hbj.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmb.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgt.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hju.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jir.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ucg.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lpk.shuidangran.top


<!-- 参考信息 -->