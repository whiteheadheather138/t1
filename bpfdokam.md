代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://zvz.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://cbk.nwbrower.top

JS:   structuredClone(obj)
来源：http://iei.nwbrower.top

TS:   structuredClone(obj)
来源：http://phh.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kas.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dle.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wtz.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ngn.smart0.xyz

[K06] 解析 URL 查询串
来源：http://tjy.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tqd.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ato.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwm.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uff.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://swj.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://egf.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://niy.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txa.ppjwa.cn

[K07] 进制转换
来源：http://con.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pha.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oug.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pmp.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lnz.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rkh.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbh.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://srg.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qsv.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://uig.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://toj.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iaa.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://jzq.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://wsy.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zpr.yj20258888.top

Go:   encoding/gob
来源：http://cei.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://lmn.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcs.cashguo.top

================================================================================
来源：http://hmg.jinqigfzy.top

L. 网络请求
来源：http://jmd.ywan-chungtsiang.top

================================================================================
来源：http://bme.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://upo.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jwx.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bal.hfpthk.cn

JS:   await fetch(url)
来源：http://efh.jqgfzy.top

TS:   await fetch(url)
来源：http://amq.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bke.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://hip.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vqi.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgb.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://amr.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://zng.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hmy.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rge.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fad.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://giq.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eyr.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uoe.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xve.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://qxt.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhe.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ume.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ata.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://icy.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qgs.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xwz.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vla.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eyh.pengpengdd.cyou

[L04] 设置超时
来源：http://cqy.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://irf.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ank.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdd.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phe.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gmi.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ifv.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jqu.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wnw.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://ayw.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tmv.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhy.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pyi.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gsh.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ywi.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mzz.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hyi.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xjp.xinyue.icu

[L06] 解析响应为 JSON
来源：http://xgt.cdnleiting.top

Py:   resp.json()
来源：http://hor.havefunace.top

PHP:  json_decode($body, true);
来源：http://htn.jqgfzy.top

JS:   await resp.json()
来源：http://ujm.bbcook.cn

TS:   await resp.json()
来源：http://san.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uhm.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tvn.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://sfv.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fqs.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://zgi.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bcr.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hea.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://tmw.yj202588.top

TS:   resp.ok;  resp.status
来源：http://ywh.tanke756.top

Java: resp.statusCode()
来源：http://bhn.yuanzhike.top

Go:   resp.StatusCode
来源：http://htp.ctjpmb.com

Ruby: resp.code.to_i
来源：http://oap.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://czj.zdqjudy.top

[L08] 并发请求多个地址
来源：http://ebg.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jri.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://wss.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://afj.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoq.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qvc.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ysp.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ynz.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://erk.zdbjq.cn

================================================================================
来源：http://ynt.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://jmv.hnxiangtu.top

================================================================================
来源：http://ifo.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://jcq.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://yrx.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://exw.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://wzj.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://wvn.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://zgj.ydzc1.top

Go:   os.Args[1:]
来源：http://mkr.vehdjk.com

Ruby: ARGV
来源：http://jra.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://akj.andypj.xyz

[M02] 读取环境变量
来源：http://sdw.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://gqv.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tpy.yangfankeji.com

JS:   process.env.HOME
来源：http://yie.9152youxi.cn

TS:   process.env.HOME
来源：http://gcj.smart0.xyz

Java: System.getenv("HOME")
来源：http://heq.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vpv.xinyue.icu

Ruby: ENV["HOME"]
来源：http://zgt.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mwe.tarul.cn

[M03] 执行外部命令
来源：http://ifj.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xsp.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dcz.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rxb.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://qts.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lix.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gll.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://shh.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://bck.vehdjk.com

[M04] 获取当前工作目录
来源：http://glu.sxryk.cn

Py:   os.getcwd()
来源：http://spe.fzhhl.top

PHP:  getcwd();
来源：http://gjq.nanxinkj.top

JS:   process.cwd()
来源：http://acr.hysaishi.cn

TS:   process.cwd()
来源：http://tmg.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://tjr.feifeiyinyue.top

Go:   os.Getwd()
来源：http://uok.sxryk.cn

Ruby: Dir.pwd
来源：http://khf.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iaa.fengsongda.top

[M05] 设置退出码
来源：http://llp.gogol.net.cn

Py:   sys.exit(1)
来源：http://fgw.smart0.xyz

PHP:  exit(1);
来源：http://iua.hcnkem.com

JS:   process.exit(1)
来源：http://afm.pengpengdd.cyou

TS:   process.exit(1)
来源：http://qev.xuetiantiany.cn

Java: System.exit(1)
来源：http://uik.yongpay.top

Go:   os.Exit(1)
来源：http://ptl.cucudq.cn

Ruby: exit 1
来源：http://zgy.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://chh.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://now.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://cvy.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ult.cheryme.top

JS:   console.error("err")
来源：http://ajk.yonumen.top

TS:   console.error("err")
来源：http://lqn.aizwys.cn

Java: System.err.println("err")
来源：http://nyl.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wgo.bbcook.cn

Ruby: warn "err"
来源：http://sub.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://saf.cashguo.top

[M07] 判断是否为主入口
来源：http://uyo.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://xgq.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pib.guannengcc.top

JS:   require.main === module
来源：http://rwa.ydjk.org.cn

TS:   require.main === module
来源：http://upf.yj20258.top

Java: public static void main(String[] args)
来源：http://yzq.zdbjq.cn

Go:   func main()
来源：http://vsc.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fql.fehbvm.com

C#:   static void Main(string[] args)
来源：http://tpi.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://qtl.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://uik.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://hff.tian-w.cn

JS:   process.platform;  process.version
来源：http://qte.chenlongwang.top

TS:   process.platform;  process.version
来源：http://ncx.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oya.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://psf.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zji.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xbm.hammf.cn

================================================================================
来源：http://pof.dashuyun.cn

N. 数据结构与算法
来源：http://vgc.jinqigfzy.top

================================================================================
来源：http://ama.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://fjt.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ktc.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oup.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbe.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vvb.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://qvg.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://cnj.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kns.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://tay.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://gdv.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://yof.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rmp.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://afe.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zyd.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggi.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://fug.zhixingplan.top

Ruby: arr.sort
来源：http://hge.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fxh.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://jtl.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zpy.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://sdh.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sxk.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zui.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://esd.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zbx.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rcs.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cdw.sweek.top

[N04] 斐波那契数列
来源：http://tnp.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hsl.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://deu.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydw.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lic.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wrj.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://orh.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xuh.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://thj.xylfe.cn

[N05] 最大公约数
来源：http://jki.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://hxk.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://krh.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oah.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kkv.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eju.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://omo.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://ntz.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kfl.xylfe.cn

[N06] 判断回文字符串
来源：http://fdw.dashuyun.cn

Py:   s == s[::-1]
来源：http://ldn.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://pfx.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://pwr.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://swu.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zdd.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://cbg.bjfxy.top

Ruby: s == s.reverse
来源：http://hsk.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iow.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://vva.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wea.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bis.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://vpb.sweek.top

TS:   // 手写 Map<string, number>
来源：http://ydy.jqgfzy.top

Java: // 手写 HashMap
来源：http://gmh.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://nci.sysykeji.top

Ruby: // 手写 Hash
来源：http://yye.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nfx.svipenyu.cn

[N08] 生成全排列
来源：http://zsl.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://xsl.wangdashe.top

PHP:  // 手写递归交换
来源：http://zoy.jyoumei.cn

JS:   // 手写回溯递归
来源：http://gqe.aibaodan.cn

TS:   // 手写回溯递归
来源：http://opz.vehdjk.com

Java: // 手写回溯递归
来源：http://sjn.guowangkeji.top

Go:   // 手写回溯递归
来源：http://btc.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://udt.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://fwm.andypj.xyz

[N09] 栈与队列
来源：http://vid.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rmm.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gso.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vpb.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jmp.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yhr.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kwg.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rsy.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ptz.yongpay.top

[N10] 链表节点定义
来源：http://ive.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hgy.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mfp.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wvy.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bog.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://jod.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://jbi.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ynm.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gpx.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://woz.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zms.yfazqb.com

PHP:  // 手写递归函数
来源：http://jmd.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqj.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qix.uphjek.com

Java: // 手写递归
来源：http://bnj.vqdsnc.cn

Go:   // 手写递归
来源：http://tbo.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ros.jianghu66.top

C#:   // 手写递归
来源：http://zmy.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vim.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zih.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://faf.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://atd.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wnz.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zpu.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bpi.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nyf.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://faf.zycfv.cn

================================================================================
来源：http://hqt.9152youxi.cn

O. 并发与异步
来源：http://yyz.xziqi.cn

================================================================================
来源：http://uvs.yj20258888.top

[O01] 启动一个线程
来源：http://jzh.shangyingyoupin.top


<!-- 参考信息 -->