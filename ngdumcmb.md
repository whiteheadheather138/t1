代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://jgh.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://efs.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hac.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rgn.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://atv.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uqu.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fyu.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vux.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://olt.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mrs.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lqz.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sbr.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xji.fktsv.cn

[K07] 进制转换
来源：http://qly.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fot.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hrh.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzj.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hya.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://myf.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://juu.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yju.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vtg.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://yyv.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://xoy.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xil.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://ymk.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://gvd.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://muj.sxryk.cn

Go:   encoding/gob
来源：http://bqc.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://hio.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnu.hywenlv.cn

================================================================================
来源：http://zdb.yj20258.top

L. 网络请求
来源：http://vwn.tanke756.top

================================================================================
来源：http://oiu.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://lyh.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rin.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xhy.shzxlz.cn

JS:   await fetch(url)
来源：http://nkj.gogol.net.cn

TS:   await fetch(url)
来源：http://wgg.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nnx.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://kjd.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://khz.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gnf.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://jdk.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://vyr.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ybd.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rbv.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wfw.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tjd.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fid.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://acg.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zyc.aizwys.cn

[L03] 设置自定义请求头
来源：http://ppq.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eig.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yam.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kwi.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlw.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awt.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://atq.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gfz.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mcf.jinyuanbaomall.cn

[L04] 设置超时
来源：http://odj.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://gbn.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tnw.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbr.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tav.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tin.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ptf.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://plw.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zam.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://zii.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ich.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rqf.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mzx.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wiz.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xbm.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mxy.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vtz.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://afq.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://mcl.zhongyouzk.top

Py:   resp.json()
来源：http://lwf.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://ugd.daria6918.cn

JS:   await resp.json()
来源：http://jyx.aibaodan.cn

TS:   await resp.json()
来源：http://xky.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pfx.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xrs.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://dno.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ilt.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://prd.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sfq.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lwr.ivvv.top

JS:   resp.ok;  resp.status
来源：http://wih.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://swr.316326.xyz

Java: resp.statusCode()
来源：http://rgf.c1oappe.top

Go:   resp.StatusCode
来源：http://qxo.cdnleiting.top

Ruby: resp.code.to_i
来源：http://bjx.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://vei.52xcode.cn

[L08] 并发请求多个地址
来源：http://fto.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hcg.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://xnd.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://loy.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpi.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xvt.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ybf.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mcd.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yyy.gzhubu.top

================================================================================
来源：http://spv.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://zcq.xuetiantiany.cn

================================================================================
来源：http://xwd.epnwcf.com

[M01] 读取命令行参数
来源：http://ssy.pycfn.com

Py:   sys.argv[1:]
来源：http://sdw.xylfe.cn

PHP:  $argv;  $argc;
来源：http://hkx.zycfv.cn

JS:   process.argv.slice(2)
来源：http://rvx.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://tdj.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://ugo.jlsjyb.cn

Go:   os.Args[1:]
来源：http://cpg.aibaodan.cn

Ruby: ARGV
来源：http://ogt.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://tei.tanke756.top

[M02] 读取环境变量
来源：http://pqe.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://wqo.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfk.hysaishi.cn

JS:   process.env.HOME
来源：http://wwo.yanxiufei.cn

TS:   process.env.HOME
来源：http://axn.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://fxc.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://chv.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://bvw.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://feo.daria6918.cn

[M03] 执行外部命令
来源：http://ujv.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fxv.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xnm.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rpw.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vrv.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://huw.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zuk.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://mvl.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://rxc.birdmap.top

[M04] 获取当前工作目录
来源：http://qss.aibaodan.cn

Py:   os.getcwd()
来源：http://xxy.uphjek.com

PHP:  getcwd();
来源：http://lww.yangfankeji.com

JS:   process.cwd()
来源：http://zva.shzxlz.cn

TS:   process.cwd()
来源：http://qka.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://cbc.hnxiangtu.top

Go:   os.Getwd()
来源：http://ems.dianchejie.cn

Ruby: Dir.pwd
来源：http://xhg.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://yyf.yangfankeji.com

[M05] 设置退出码
来源：http://xtc.hnqzz.top

Py:   sys.exit(1)
来源：http://ccg.vehdjk.com

PHP:  exit(1);
来源：http://iwf.guowangkeji.top

JS:   process.exit(1)
来源：http://dld.52xcode.cn

TS:   process.exit(1)
来源：http://atq.xylfe.cn

Java: System.exit(1)
来源：http://esp.birdmap.top

Go:   os.Exit(1)
来源：http://xnq.yonumen.top

Ruby: exit 1
来源：http://eef.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://arh.jiagoushi.top

[M06] 向标准错误输出
来源：http://ylq.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://ush.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://knj.hywenlv.cn

JS:   console.error("err")
来源：http://ouj.sysykeji.top

TS:   console.error("err")
来源：http://shm.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://agu.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ooh.guowangkeji.top

Ruby: warn "err"
来源：http://zjg.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://fzl.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://cwy.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://qxk.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ilw.sxryk.cn

JS:   require.main === module
来源：http://tqv.fzhhl.top

TS:   require.main === module
来源：http://jef.zdqjudy.top

Java: public static void main(String[] args)
来源：http://fjs.zhoulong.xyz

Go:   func main()
来源：http://lfx.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yyc.yj20258.top

C#:   static void Main(string[] args)
来源：http://zfh.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://xzx.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://rdp.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://xku.tanke756.top

JS:   process.platform;  process.version
来源：http://ouc.jqgfzy.top

TS:   process.platform;  process.version
来源：http://ebh.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vcu.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gbi.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wru.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jte.tianlin.xyz

================================================================================
来源：http://biy.zycfv.cn

N. 数据结构与算法
来源：http://kpy.yongpay.top

================================================================================
来源：http://xla.uphjek.com

[N01] 二分查找（有序数组）
来源：http://ick.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lmj.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pqf.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ker.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlj.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nsh.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://lfz.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mfu.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://ram.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://ejf.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://ydj.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gnh.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ils.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zbc.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mau.yj202588.top

Go:   slices.Sort(arr)
来源：http://suz.gzhubu.top

Ruby: arr.sort
来源：http://ggd.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://fsf.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://xrc.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xqd.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://oqj.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ceg.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjv.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fxl.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://odz.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://adv.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cfq.fengsongda.top

[N04] 斐波那契数列
来源：http://xmh.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qep.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kss.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://akt.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdv.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uxs.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cfw.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nmp.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ftk.haohaochexian.top

[N05] 最大公约数
来源：http://wts.yvedp.cn

Py:   math.gcd(a, b)
来源：http://swk.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://viq.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgs.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxv.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oxu.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uyd.yuanzhike.top

Ruby: a.gcd(b)
来源：http://gpc.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jrl.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://ddn.zhongyouzk.top

Py:   s == s[::-1]
来源：http://gos.c1oappe.top

PHP:  $s === strrev($s);
来源：http://ikh.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://tpw.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://xtl.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://upl.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://xbz.hcnkem.com

Ruby: s == s.reverse
来源：http://mfp.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kns.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://ymi.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pdq.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qrm.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://olv.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://yeg.sweek.top

Java: // 手写 HashMap
来源：http://spk.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://muy.zdqjudy.top

Ruby: // 手写 Hash
来源：http://ohg.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pef.yanxiufei.cn

[N08] 生成全排列
来源：http://rnt.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://acp.aibaodan.cn

PHP:  // 手写递归交换
来源：http://gdu.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://stu.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://sex.andypj.xyz

Java: // 手写回溯递归
来源：http://jzx.yueranfly.top

Go:   // 手写回溯递归
来源：http://yvl.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://agg.c1oappe.top

C#:   // 手写回溯递归
来源：http://vbo.shuidangran.top

[N09] 栈与队列
来源：http://lic.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://abh.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ooj.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://igw.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cjy.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hks.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xel.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rel.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lvp.gotoacloud.top

[N10] 链表节点定义
来源：http://adh.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xhq.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uyq.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tmi.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yrq.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://zcn.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://leh.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uex.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://gbz.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://bjm.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pgh.gogol.net.cn

PHP:  // 手写递归函数
来源：http://qzh.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tot.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwf.vehdjk.com

Java: // 手写递归
来源：http://qlq.smart0.xyz

Go:   // 手写递归
来源：http://vhw.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dkj.birdmap.top

C#:   // 手写递归
来源：http://lhz.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fsm.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://drd.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qea.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ihf.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozg.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hco.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ygf.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nbu.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vvk.havefunace.top

================================================================================
来源：http://dbz.daxiang520.top

O. 并发与异步
来源：http://jwa.nwbrower.top

================================================================================
来源：http://eer.fengsongda.top

[O01] 启动一个线程
来源：http://dez.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tvr.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nyt.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uyl.kuanghao11.cn

TS:   // 同 JS
来源：http://rmd.yanxiufei.cn


<!-- 参考信息 -->