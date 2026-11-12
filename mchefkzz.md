代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://nxi.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://lwy.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://eqp.tanke756.top

TS:   structuredClone(obj)
来源：http://nem.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wqs.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uvs.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxs.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://imz.yonumen.top

[K06] 解析 URL 查询串
来源：http://neg.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ckw.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iqb.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fiv.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gkj.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uhv.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hfs.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdx.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aui.yueranfly.top

[K07] 进制转换
来源：http://uzs.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ixp.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oda.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lsv.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yee.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wje.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vvn.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qhd.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kud.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://qnx.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://sgx.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mjo.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://jxb.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://beh.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oqg.vqdsnc.cn

Go:   encoding/gob
来源：http://mii.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://bkp.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mxp.nwbrower.top

================================================================================
来源：http://snt.uphjek.com

L. 网络请求
来源：http://xng.sysykeji.top

================================================================================
来源：http://ipg.ctjpmb.com

[L01] 发送 GET 请求
来源：http://zyx.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wyg.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ikk.yuxming.cn

JS:   await fetch(url)
来源：http://egm.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://bng.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://siy.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://irm.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://phk.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gji.xylfe.cn

[L02] 发送 POST JSON
来源：http://fyx.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://apd.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pjn.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oeb.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojo.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gxh.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ato.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iey.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vai.yueranfly.top

[L03] 设置自定义请求头
来源：http://tie.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxg.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zpp.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cux.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kik.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://asf.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ndw.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ppj.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysw.fehbvm.com

[L04] 设置超时
来源：http://yww.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://ynv.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kqk.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyd.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nkv.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://waz.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://irl.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yev.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://buv.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://zfa.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xaw.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sda.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://odh.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mnd.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ito.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://man.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sjh.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npq.hammf.cn

[L06] 解析响应为 JSON
来源：http://esv.fanxiaobao.xyz

Py:   resp.json()
来源：http://fra.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://mas.shanyushiyangtech.top

JS:   await resp.json()
来源：http://wwi.jqgfzy.top

TS:   await resp.json()
来源：http://biq.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ziz.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iaf.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://joq.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbx.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://rkp.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ekv.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vxv.tanke756.top

JS:   resp.ok;  resp.status
来源：http://eia.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://ghs.cheryme.top

Java: resp.statusCode()
来源：http://ncd.ydzc1.top

Go:   resp.StatusCode
来源：http://kkw.tarul.cn

Ruby: resp.code.to_i
来源：http://xmt.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://zeu.zdbjq.cn

[L08] 并发请求多个地址
来源：http://ouk.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sus.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://dxs.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nya.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ehw.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cms.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hod.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lgf.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xsu.tian-w.cn

================================================================================
来源：http://pxw.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://cow.snrcjt.cn

================================================================================
来源：http://frj.cucudq.cn

[M01] 读取命令行参数
来源：http://eak.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://rnt.daxiang520.top

PHP:  $argv;  $argc;
来源：http://hyb.xinyue.icu

JS:   process.argv.slice(2)
来源：http://xyd.tanke756.top

TS:   process.argv.slice(2)
来源：http://gvx.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://qdl.birdmap.top

Go:   os.Args[1:]
来源：http://dkz.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://jui.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://mjt.cheryme.top

[M02] 读取环境变量
来源：http://cul.havefunace.top

Py:   os.environ.get("HOME")
来源：http://udz.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sla.cqqwz.cn

JS:   process.env.HOME
来源：http://zdt.shuidangran.top

TS:   process.env.HOME
来源：http://ojw.yueranfly.top

Java: System.getenv("HOME")
来源：http://jjs.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvk.fehbvm.com

Ruby: ENV["HOME"]
来源：http://nrx.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jeg.shuidangran.top

[M03] 执行外部命令
来源：http://qxf.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ats.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qhi.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://ngn.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bzl.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hyn.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ycj.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://bul.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://esi.dianchejie.cn

[M04] 获取当前工作目录
来源：http://yjh.jqgufenzy.top

Py:   os.getcwd()
来源：http://lem.hnxiangtu.top

PHP:  getcwd();
来源：http://hoj.ivvv.top

JS:   process.cwd()
来源：http://mqp.shuidangran.top

TS:   process.cwd()
来源：http://pzv.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://zub.xziqi.cn

Go:   os.Getwd()
来源：http://hgc.bjfxy.top

Ruby: Dir.pwd
来源：http://sak.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pel.svipenyu.cn

[M05] 设置退出码
来源：http://zye.zhengqikj.top

Py:   sys.exit(1)
来源：http://ebj.zhoulong.xyz

PHP:  exit(1);
来源：http://uyn.snrcjt.cn

JS:   process.exit(1)
来源：http://qqq.tarul.cn

TS:   process.exit(1)
来源：http://cvq.gotoacloud.top

Java: System.exit(1)
来源：http://bij.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://bly.epnwcf.com

Ruby: exit 1
来源：http://hoz.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwt.0kj1m.cn

[M06] 向标准错误输出
来源：http://auq.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://lep.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iev.shanyushiyangtech.top

JS:   console.error("err")
来源：http://qka.ivvv.top

TS:   console.error("err")
来源：http://vma.sufxvd.cn

Java: System.err.println("err")
来源：http://tzs.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ror.yfazqb.com

Ruby: warn "err"
来源：http://hin.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://gdl.xylfe.cn

[M07] 判断是否为主入口
来源：http://cdv.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://lkm.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fhq.yangfankeji.com

JS:   require.main === module
来源：http://wun.sufxvd.cn

TS:   require.main === module
来源：http://zaf.bjfxy.top

Java: public static void main(String[] args)
来源：http://nmz.52xcode.cn

Go:   func main()
来源：http://lck.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cnb.hnqzz.top

C#:   static void Main(string[] args)
来源：http://zzp.pycfn.com

[M08] 获取系统与运行时信息
来源：http://thi.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://dry.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://whq.hysaishi.cn

JS:   process.platform;  process.version
来源：http://fyk.epnwcf.com

TS:   process.platform;  process.version
来源：http://hkj.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nby.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rol.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gew.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mnj.ybcxt.top

================================================================================
来源：http://igh.ybcxt.top

N. 数据结构与算法
来源：http://mma.ppjwa.cn

================================================================================
来源：http://pyq.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://tmo.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zvq.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rke.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqp.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vwg.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://nwi.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://pjj.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uws.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://yea.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rqr.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://cbw.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clb.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpq.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryk.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dhl.havefunace.top

Go:   slices.Sort(arr)
来源：http://lxx.birdmap.top

Ruby: arr.sort
来源：http://bce.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rbo.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://rbe.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uzi.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://hzu.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xhq.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mht.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ksu.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qzq.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tvx.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://qru.chenzaomai.com

[N04] 斐波那契数列
来源：http://vja.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxu.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eym.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xmu.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhs.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zgt.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nsq.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://raf.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://leh.daria6918.cn

[N05] 最大公约数
来源：http://cda.ybcxt.top

Py:   math.gcd(a, b)
来源：http://obx.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ikc.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avb.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://juk.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qgv.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qdx.snrcjt.cn

Ruby: a.gcd(b)
来源：http://fzq.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tgp.bbcook.cn

[N06] 判断回文字符串
来源：http://eqj.smart0.xyz

Py:   s == s[::-1]
来源：http://ocw.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://hdj.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://xcg.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://vfk.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bhp.tian-w.cn

Go:   // 双指针从两端比较
来源：http://tjy.wangdashe.top

Ruby: s == s.reverse
来源：http://lrk.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uls.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://tir.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pod.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jkr.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ybx.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://xbc.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://sin.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://ksp.wangdashe.top

Ruby: // 手写 Hash
来源：http://rqj.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://xpy.zdqjudy.top

[N08] 生成全排列
来源：http://hap.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://jlz.ctjpmb.com

PHP:  // 手写递归交换
来源：http://ibi.shzxlz.cn

JS:   // 手写回溯递归
来源：http://myj.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://arh.yj20258.top

Java: // 手写回溯递归
来源：http://mba.pycfn.com

Go:   // 手写回溯递归
来源：http://rpj.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://wvw.jianghu66.top

C#:   // 手写回溯递归
来源：http://yiv.xuetiantiany.cn

[N09] 栈与队列
来源：http://nkt.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fth.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://phx.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pnl.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kss.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xue.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zoq.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mut.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sbb.ybcxt.top

[N10] 链表节点定义
来源：http://smr.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ejw.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cfl.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eph.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wqr.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://kxx.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://laq.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bcn.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kqw.epnwcf.com

[N11] 二叉树中序遍历
来源：http://jxe.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hsb.cdnleiting.top

PHP:  // 手写递归函数
来源：http://xti.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wke.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ejl.ehwqpu.com

Java: // 手写递归
来源：http://upq.zycfv.cn

Go:   // 手写递归
来源：http://imm.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wlq.tarul.cn

C#:   // 手写递归
来源：http://tkz.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ize.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szp.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wnb.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://byg.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fdw.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhe.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jhv.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aox.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://udb.dashuyun.cn

================================================================================
来源：http://loy.ydzc1.top

O. 并发与异步
来源：http://vdz.chenzaomai.com

================================================================================
来源：http://dxl.cdnleiting.top

[O01] 启动一个线程
来源：http://xxa.havefunace.top


<!-- 参考信息 -->