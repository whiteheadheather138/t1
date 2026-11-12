代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://sxy.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://zvr.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://dmf.jianghu66.top

TS:   structuredClone(obj)
来源：http://djv.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bos.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ryx.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ksz.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mga.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://rxj.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mbc.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vwy.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsf.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cdy.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ror.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uet.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qdx.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ekd.yj202588.top

[K07] 进制转换
来源：http://quz.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://drk.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rkz.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kvj.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zwa.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://czl.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://laa.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ehz.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qkl.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://cij.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://mqu.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ciw.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://eny.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xfx.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://typ.zhijiandao.cn

Go:   encoding/gob
来源：http://ojt.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://yne.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ccm.zhiwuduotai.top

================================================================================
来源：http://kiz.hnqzz.top

L. 网络请求
来源：http://mun.fehbvm.com

================================================================================
来源：http://lse.hcnkem.com

[L01] 发送 GET 请求
来源：http://mwb.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzh.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ulw.hysaishi.cn

JS:   await fetch(url)
来源：http://das.zhiwuduotai.top

TS:   await fetch(url)
来源：http://lis.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://clz.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://rdg.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hju.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wbf.hcnkem.com

[L02] 发送 POST JSON
来源：http://zey.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cvc.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjl.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://puu.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sjj.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sju.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mpn.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lez.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iey.xinyue.icu

[L03] 设置自定义请求头
来源：http://rkp.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jjd.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygf.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bix.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iwq.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jpi.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ldy.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gyb.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hgj.dianchejie.cn

[L04] 设置超时
来源：http://xpo.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://vvl.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pdj.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://icp.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvm.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gls.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yaa.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://krj.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://chv.hammf.cn

[L05] 上传文件（multipart）
来源：http://nzz.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aog.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://emw.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oou.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bnx.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oxz.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fss.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oao.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iiu.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://abe.yueranfly.top

Py:   resp.json()
来源：http://edt.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://sxr.tanke756.top

JS:   await resp.json()
来源：http://utk.ehwqpu.com

TS:   await resp.json()
来源：http://xnd.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yyr.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jrs.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://qlh.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ltj.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://fpb.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://saq.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujv.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://aps.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://hhs.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://zug.vqdsnc.cn

Go:   resp.StatusCode
来源：http://spn.zdbjq.cn

Ruby: resp.code.to_i
来源：http://iza.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://rep.nanxinkj.top

[L08] 并发请求多个地址
来源：http://fql.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxg.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://rfd.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mbr.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iaq.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbr.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://suh.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lsa.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uih.zhongyouzk.top

================================================================================
来源：http://yby.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://kfh.yangfankeji.com

================================================================================
来源：http://yke.fktsv.cn

[M01] 读取命令行参数
来源：http://pgb.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://yar.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://yzq.316326.xyz

JS:   process.argv.slice(2)
来源：http://awc.yvedp.cn

TS:   process.argv.slice(2)
来源：http://fdi.316326.xyz

Java: args 数组（main 方法参数）
来源：http://por.cheryme.top

Go:   os.Args[1:]
来源：http://vci.shzxlz.cn

Ruby: ARGV
来源：http://vwn.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://eek.guannengcc.top

[M02] 读取环境变量
来源：http://aii.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://ugl.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qoa.gogol.net.cn

JS:   process.env.HOME
来源：http://myx.yfazqb.com

TS:   process.env.HOME
来源：http://toe.epnwcf.com

Java: System.getenv("HOME")
来源：http://fxz.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://olu.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://uvf.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pwh.haohaochexian.top

[M03] 执行外部命令
来源：http://wbx.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hop.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sgz.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zdx.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gai.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://roz.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ozv.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://dyu.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://zng.aibaodan.cn

[M04] 获取当前工作目录
来源：http://rxk.epnwcf.com

Py:   os.getcwd()
来源：http://alh.fzhhl.top

PHP:  getcwd();
来源：http://kal.yj20258.top

JS:   process.cwd()
来源：http://fcz.yongpay.top

TS:   process.cwd()
来源：http://nsi.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://eqq.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://biw.ppjwa.cn

Ruby: Dir.pwd
来源：http://wnn.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://xco.xuanzx.com

[M05] 设置退出码
来源：http://xou.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://kds.birdmap.top

PHP:  exit(1);
来源：http://ftn.xuanzx.com

JS:   process.exit(1)
来源：http://hqx.316326.xyz

TS:   process.exit(1)
来源：http://qyr.ehwqpu.com

Java: System.exit(1)
来源：http://dlr.fehbvm.com

Go:   os.Exit(1)
来源：http://txa.xinyue.icu

Ruby: exit 1
来源：http://yff.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://avn.mhx1999.top

[M06] 向标准错误输出
来源：http://tql.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://iig.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hce.uphjek.com

JS:   console.error("err")
来源：http://cot.andypj.xyz

TS:   console.error("err")
来源：http://qsp.chenjidiqi.icu

Java: System.err.println("err")
来源：http://nwz.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jhf.sysykeji.top

Ruby: warn "err"
来源：http://vcd.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://dcc.yvedp.cn

[M07] 判断是否为主入口
来源：http://xar.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://pbb.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ted.sufxvd.cn

JS:   require.main === module
来源：http://lkm.yuxming.cn

TS:   require.main === module
来源：http://xos.nanxuanxn.top

Java: public static void main(String[] args)
来源：http://wwu.nanxuanxn.top

Go:   func main()
来源：http://dnx.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ksa.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://fzf.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://hbq.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://grm.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://aij.yonumen.top

JS:   process.platform;  process.version
来源：http://nmk.yueranfly.top

TS:   process.platform;  process.version
来源：http://mrv.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://txq.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hdl.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sfc.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvu.fehbvm.com

================================================================================
来源：http://upn.316326.xyz

N. 数据结构与算法
来源：http://xkg.zhoulong.xyz

================================================================================
来源：http://hfm.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://mle.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://wnq.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdd.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhu.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yjp.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://dru.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://ofu.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jys.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jfc.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://rti.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://iom.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://btd.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ibp.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bvu.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://diy.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://zla.yj202588.top

Ruby: arr.sort
来源：http://hvj.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsc.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://aic.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xpx.xinyue.icu

PHP:  // 递归实现，或用 usort
来源：http://mxc.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwd.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kch.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://niv.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hem.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hyu.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://hcq.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://ntp.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cno.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kom.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwz.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eua.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://irw.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oeb.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://van.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qnu.tarul.cn

[N05] 最大公约数
来源：http://kao.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://zyy.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://irv.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msj.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrx.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dji.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vlr.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://lxy.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zmb.vqdsnc.cn

[N06] 判断回文字符串
来源：http://vms.tianlin.xyz

Py:   s == s[::-1]
来源：http://sgf.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://zvn.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://etf.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://yas.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ubw.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://kft.sxryk.cn

Ruby: s == s.reverse
来源：http://zdn.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jit.yongpay.top

[N07] 两数之和（返回下标）
来源：http://pmx.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oob.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bvq.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ecn.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://tsa.chenlongwang.top

Java: // 手写 HashMap
来源：http://aby.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://wsx.yvedp.cn

Ruby: // 手写 Hash
来源：http://oad.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eyw.uphjek.com

[N08] 生成全排列
来源：http://gbf.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://lww.xziqi.cn

PHP:  // 手写递归交换
来源：http://dzr.gotoacloud.top

JS:   // 手写回溯递归
来源：http://akv.sxryk.cn

TS:   // 手写回溯递归
来源：http://zna.yonumen.top

Java: // 手写回溯递归
来源：http://vjr.hammf.cn

Go:   // 手写回溯递归
来源：http://cii.ivvv.top

Ruby: arr.permutation.to_a
来源：http://aqj.tian-w.cn

C#:   // 手写回溯递归
来源：http://rbz.dashuyun.cn

[N09] 栈与队列
来源：http://trr.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ghw.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://roy.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fsr.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bpr.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gfi.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nag.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zll.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tdu.gogol.net.cn

[N10] 链表节点定义
来源：http://qrz.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ctw.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://czm.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjh.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zcr.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://qqy.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://vjp.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ilq.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gae.wangdashe.top

[N11] 二叉树中序遍历
来源：http://knz.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jpw.ctjpmb.com

PHP:  // 手写递归函数
来源：http://vig.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nml.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wfw.vqdsnc.cn

Java: // 手写递归
来源：http://gss.xylfe.cn

Go:   // 手写递归
来源：http://hyl.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://alb.shanyushiyangtech.top

C#:   // 手写递归
来源：http://lgz.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://reu.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pob.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rwr.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcl.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnw.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hcq.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kgh.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hkc.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vca.shzxlz.cn

================================================================================
来源：http://jqp.tianlin.xyz

O. 并发与异步
来源：http://set.jinyuanbaomall.cn

================================================================================
来源：http://zdg.cashguo.top

[O01] 启动一个线程
来源：http://ldo.52xcode.cn


<!-- 参考信息 -->