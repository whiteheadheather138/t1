代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gyu.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uho.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvi.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://zhy.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://hdr.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://bzr.xuanzx.com

JS:   structuredClone(obj)
来源：http://amq.cheryme.top

TS:   structuredClone(obj)
来源：http://dsk.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pcq.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ift.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgy.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://czg.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://lwv.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://enh.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dja.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ehd.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://coi.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mve.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jgk.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fnn.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://djs.sufxvd.cn

[K07] 进制转换
来源：http://fqc.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bfq.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://khu.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://axx.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mln.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jjm.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oae.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kvd.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gii.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://jcx.pycfn.com

Py:   pickle.dumps(obj)
来源：http://fwi.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vil.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://wug.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://wjm.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fxx.tarul.cn

Go:   encoding/gob
来源：http://tzz.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://ekn.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zwl.zhaomingkeji.xyz

================================================================================
来源：http://ype.sxryk.cn

L. 网络请求
来源：http://kbx.shuidangran.top

================================================================================
来源：http://via.aibaodan.cn

[L01] 发送 GET 请求
来源：http://xnf.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pyu.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bfl.haohaochexian.top

JS:   await fetch(url)
来源：http://chh.cashguo.top

TS:   await fetch(url)
来源：http://fbn.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yyr.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://eqo.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://eub.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mgp.cqqwz.cn

[L02] 发送 POST JSON
来源：http://ezr.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://noi.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qtp.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pfh.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jee.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kao.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lcq.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ijg.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cmc.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://nzq.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://esb.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dkc.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgh.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://phe.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zcl.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yqs.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alp.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xkk.zhiwuduotai.top

[L04] 设置超时
来源：http://mov.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://qhq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oge.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://luw.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://llz.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lqy.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://daq.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mnp.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hdw.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://tpc.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://opo.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://imq.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://usz.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mxi.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cjy.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://swq.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rvc.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iey.iojbl.cn

[L06] 解析响应为 JSON
来源：http://hml.0kj1m.cn

Py:   resp.json()
来源：http://oqn.gzhubu.top

PHP:  json_decode($body, true);
来源：http://tya.feifeiyinyue.top

JS:   await resp.json()
来源：http://nib.ctjpmb.com

TS:   await resp.json()
来源：http://utn.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mhz.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lnz.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://egw.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xxr.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://xoj.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fnx.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://toj.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://ept.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://hjo.ctjpmb.com

Java: resp.statusCode()
来源：http://esb.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://fmy.9152youxi.cn

Ruby: resp.code.to_i
来源：http://bmr.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://gpf.pycfn.com

[L08] 并发请求多个地址
来源：http://mkz.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pui.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://zsz.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wid.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wiq.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ksl.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://urn.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qmr.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dtv.hongshengwenyu.top

================================================================================
来源：http://kzr.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://sda.zycfv.cn

================================================================================
来源：http://wli.zhengqikj.top

[M01] 读取命令行参数
来源：http://aqs.uphjek.com

Py:   sys.argv[1:]
来源：http://tcf.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://vyy.aizwys.cn

JS:   process.argv.slice(2)
来源：http://xds.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://wmo.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://ose.zycfv.cn

Go:   os.Args[1:]
来源：http://gnp.nanxinkj.top

Ruby: ARGV
来源：http://lhw.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://mlx.sweek.top

[M02] 读取环境变量
来源：http://ajv.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://paa.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rao.zdbjq.cn

JS:   process.env.HOME
来源：http://enc.chenjidiqi.icu

TS:   process.env.HOME
来源：http://huv.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://ufy.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qvy.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://ief.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nne.wangdashe.top

[M03] 执行外部命令
来源：http://kka.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tgl.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wcq.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hkt.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mox.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://duw.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yvd.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://gxt.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://kfe.daria6918.cn

[M04] 获取当前工作目录
来源：http://rcc.snrcjt.cn

Py:   os.getcwd()
来源：http://ikg.ybcxt.top

PHP:  getcwd();
来源：http://ube.shangyingyoupin.top

JS:   process.cwd()
来源：http://wua.shzxlz.cn

TS:   process.cwd()
来源：http://tgi.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://hkm.smart0.xyz

Go:   os.Getwd()
来源：http://yyq.guowangkeji.top

Ruby: Dir.pwd
来源：http://hek.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://dyg.mhx1999.top

[M05] 设置退出码
来源：http://uaf.snrcjt.cn

Py:   sys.exit(1)
来源：http://oli.sysykeji.top

PHP:  exit(1);
来源：http://jbi.shuidangran.top

JS:   process.exit(1)
来源：http://xnt.yuanzhike.top

TS:   process.exit(1)
来源：http://hio.zhixingplan.top

Java: System.exit(1)
来源：http://jso.tian-w.cn

Go:   os.Exit(1)
来源：http://atq.guannengcc.top

Ruby: exit 1
来源：http://wln.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gam.yueranfly.top

[M06] 向标准错误输出
来源：http://aob.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://ctt.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ipw.yanxiufei.cn

JS:   console.error("err")
来源：http://upb.52xcode.cn

TS:   console.error("err")
来源：http://flj.jianghu66.top

Java: System.err.println("err")
来源：http://fpz.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dcp.hysaishi.cn

Ruby: warn "err"
来源：http://qmv.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://gqf.c1oappe.top

[M07] 判断是否为主入口
来源：http://zxh.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://ppy.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hgo.sjlbkw.cn

JS:   require.main === module
来源：http://qum.fktsv.cn

TS:   require.main === module
来源：http://hbp.hammf.cn

Java: public static void main(String[] args)
来源：http://hyl.hywenlv.cn

Go:   func main()
来源：http://vxv.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://doo.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://ytk.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://uac.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://bav.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://haq.jianghu66.top

JS:   process.platform;  process.version
来源：http://uad.xziqi.cn

TS:   process.platform;  process.version
来源：http://wpq.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ncj.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sjm.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kql.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ekb.ehwqpu.com

================================================================================
来源：http://bdy.zhongyouzk.top

N. 数据结构与算法
来源：http://igq.nanxinkj.top

================================================================================
来源：http://ujp.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://rfu.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oqp.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oax.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lao.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwu.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://gfg.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://emi.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://uvh.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://eqh.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://cbq.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://eah.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://duc.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uwy.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iwr.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xtd.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://ttg.sxryk.cn

Ruby: arr.sort
来源：http://mua.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://voa.yj20258.top

[N03] 快速排序（分治示例）
来源：http://cil.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qxk.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://zjo.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogg.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aop.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xne.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxy.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jnk.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kaj.zhijiandao.cn

[N04] 斐波那契数列
来源：http://cbq.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rfg.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dqx.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epi.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gfz.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kol.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pcm.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hcg.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zpj.bbcook.cn

[N05] 最大公约数
来源：http://fcn.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://eaw.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wgx.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obc.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fum.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jvv.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixj.c1oappe.top

Ruby: a.gcd(b)
来源：http://xwd.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hdj.mhx1999.top

[N06] 判断回文字符串
来源：http://iix.jinqigfzy.top

Py:   s == s[::-1]
来源：http://lcj.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://ujm.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://dma.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://lbm.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://usr.yj20258888.top

Go:   // 双指针从两端比较
来源：http://muz.zhijiandao.cn

Ruby: s == s.reverse
来源：http://ioq.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://whu.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://yiq.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sne.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eha.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zjp.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://vaz.tian-w.cn

Java: // 手写 HashMap
来源：http://iyl.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://whg.hywenlv.cn

Ruby: // 手写 Hash
来源：http://iwn.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wor.c1oappe.top

[N08] 生成全排列
来源：http://jwn.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://wkd.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://sho.uphjek.com

JS:   // 手写回溯递归
来源：http://tnv.c1oappe.top

TS:   // 手写回溯递归
来源：http://qkt.52xcode.cn

Java: // 手写回溯递归
来源：http://yli.yj20258.top

Go:   // 手写回溯递归
来源：http://eqj.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://bil.tarul.cn

C#:   // 手写回溯递归
来源：http://rrp.xuetiantiany.cn

[N09] 栈与队列
来源：http://tbr.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zmy.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tdu.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkj.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://adl.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kbs.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jsd.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vwv.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iko.jqgufenzy.top

[N10] 链表节点定义
来源：http://ppd.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://adm.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kle.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bly.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zbo.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://zui.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://uar.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://syr.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gak.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://qmh.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lfm.iojbl.cn

PHP:  // 手写递归函数
来源：http://dby.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://his.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kic.guowangkeji.top

Java: // 手写递归
来源：http://jcs.zhengqikj.top

Go:   // 手写递归
来源：http://ojl.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://keo.jiagoushi.top

C#:   // 手写递归
来源：http://gli.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zbp.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://goi.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vzz.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wog.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cvy.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nwh.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fnd.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mcr.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fgk.0kj1m.cn


<!-- 参考信息 -->