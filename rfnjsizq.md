代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://haq.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://big.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xgp.chenzaomai.com

[K05] 深拷贝对象
来源：http://lxn.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://ycy.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://uyl.snrcjt.cn

JS:   structuredClone(obj)
来源：http://tsd.gogol.net.cn

TS:   structuredClone(obj)
来源：http://qve.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://vza.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zxj.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://itv.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sji.zycfv.cn

[K06] 解析 URL 查询串
来源：http://lha.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qnk.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dac.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egh.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://meu.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tzx.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://myd.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wsd.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ize.chenlongwang.top

[K07] 进制转换
来源：http://wfq.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ncr.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qxg.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jjr.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pmf.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eao.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://njx.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://axi.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rac.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://hzn.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://qkh.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rhd.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://dtl.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://jah.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pwk.guowangkeji.top

Go:   encoding/gob
来源：http://qtq.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://xgi.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvs.hammf.cn

================================================================================
来源：http://smx.xuetiantiany.cn

L. 网络请求
来源：http://cwn.quarkkingdee.top

================================================================================
来源：http://khy.aibaodan.cn

[L01] 发送 GET 请求
来源：http://yah.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hur.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vcz.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://bdu.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://ozw.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gyg.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://oss.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pcl.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eju.ctjpmb.com

[L02] 发送 POST JSON
来源：http://kyz.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://qya.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ndd.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxs.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxw.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ddq.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rhj.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqx.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cyi.snrcjt.cn

[L03] 设置自定义请求头
来源：http://ynf.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrm.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tdu.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ama.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqo.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tba.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ufz.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cox.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mde.meibo888.top

[L04] 设置超时
来源：http://zsp.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://thr.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kzo.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdt.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjy.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xfv.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vnx.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qol.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sgp.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://xqo.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://npf.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aoy.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gxe.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tod.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xum.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ycz.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zvm.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://igf.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://bkm.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://iwe.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://ynh.aizwys.cn

JS:   await resp.json()
来源：http://bgv.svipenyu.cn

TS:   await resp.json()
来源：http://lvg.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fiz.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zix.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://rbj.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gun.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://hcy.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wao.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dan.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://ewf.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://rqi.fktsv.cn

Java: resp.statusCode()
来源：http://myq.sxryk.cn

Go:   resp.StatusCode
来源：http://dpb.nwbrower.top

Ruby: resp.code.to_i
来源：http://fgj.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://irq.sweek.top

[L08] 并发请求多个地址
来源：http://nph.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cbk.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://vwu.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbx.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdx.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xwe.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbd.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cop.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hjl.jinqigfzy.top

================================================================================
来源：http://czi.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://rvw.jlsjyb.cn

================================================================================
来源：http://fjg.yuxming.cn

[M01] 读取命令行参数
来源：http://rkx.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://kzb.daxiang520.top

PHP:  $argv;  $argc;
来源：http://sxo.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://duq.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://zov.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://igc.snrcjt.cn

Go:   os.Args[1:]
来源：http://pdb.guowangkeji.top

Ruby: ARGV
来源：http://xpr.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://oho.ppjwa.cn

[M02] 读取环境变量
来源：http://whr.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://kxu.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tgi.nanxuanxn.top

JS:   process.env.HOME
来源：http://yzo.c1oappe.top

TS:   process.env.HOME
来源：http://okt.cashguo.top

Java: System.getenv("HOME")
来源：http://paa.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://frj.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://xec.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://utl.vqdsnc.cn

[M03] 执行外部命令
来源：http://ykp.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uxf.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fwl.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lyf.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://asc.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mro.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://mks.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://wca.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://dvp.tarul.cn

[M04] 获取当前工作目录
来源：http://bwr.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://yts.feifeiyinyue.top

PHP:  getcwd();
来源：http://dgb.ehwqpu.com

JS:   process.cwd()
来源：http://rns.yuxming.cn

TS:   process.cwd()
来源：http://vgk.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://dmm.jianghu66.top

Go:   os.Getwd()
来源：http://pix.gzhubu.top

Ruby: Dir.pwd
来源：http://avc.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://azf.gogol.net.cn

[M05] 设置退出码
来源：http://rkh.gogol.net.cn

Py:   sys.exit(1)
来源：http://tuf.zycfv.cn

PHP:  exit(1);
来源：http://xyq.aibaodan.cn

JS:   process.exit(1)
来源：http://jwu.zhoulong.xyz

TS:   process.exit(1)
来源：http://xko.zycfv.cn

Java: System.exit(1)
来源：http://zpy.gogol.net.cn

Go:   os.Exit(1)
来源：http://onu.daria6918.cn

Ruby: exit 1
来源：http://cgp.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfb.0kj1m.cn

[M06] 向标准错误输出
来源：http://wwt.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://exj.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sbv.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://rxr.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://kob.gotoacloud.top

Java: System.err.println("err")
来源：http://ycf.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsa.tarul.cn

Ruby: warn "err"
来源：http://nqf.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://ozd.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://gog.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://cbi.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdx.wangdashe.top

JS:   require.main === module
来源：http://xfm.nwbrower.top

TS:   require.main === module
来源：http://pvd.jqgfzy.top

Java: public static void main(String[] args)
来源：http://utz.ehwqpu.com

Go:   func main()
来源：http://wzz.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://foi.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://qdv.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://bnj.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://eaj.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ebh.hammf.cn

JS:   process.platform;  process.version
来源：http://lha.jinqigufen.top

TS:   process.platform;  process.version
来源：http://eok.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ent.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://quw.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fyt.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ivh.shanyushiyangkeji.top

================================================================================
来源：http://zle.guowangkeji.top

N. 数据结构与算法
来源：http://mff.yj20258.top

================================================================================
来源：http://evl.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://coo.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://hte.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lra.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ozk.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kst.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://qhq.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://zpu.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://coi.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lyi.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://ekj.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://lmh.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hza.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://mon.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ngk.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ays.smart0.xyz

Go:   slices.Sort(arr)
来源：http://xpf.epnwcf.com

Ruby: arr.sort
来源：http://rly.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://irb.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://fsm.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aop.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://abn.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uxk.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sbu.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ftd.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dkt.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vdh.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://tev.jiagoushi.top

[N04] 斐波那契数列
来源：http://phb.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kkl.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psf.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://avu.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uik.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gpm.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cdj.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kjx.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hdv.vehdjk.com

[N05] 最大公约数
来源：http://kji.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://hsz.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zed.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jnf.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wwu.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cza.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsz.nwbrower.top

Ruby: a.gcd(b)
来源：http://nca.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbx.cheryme.top

[N06] 判断回文字符串
来源：http://bhu.havefunace.top

Py:   s == s[::-1]
来源：http://ghx.gzhubu.top

PHP:  $s === strrev($s);
来源：http://bcs.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://hgy.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://ekl.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gpo.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://rma.sweek.top

Ruby: s == s.reverse
来源：http://zat.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://aol.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://vnu.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hul.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://quq.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kym.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://tis.gaohongyu789.top

Java: // 手写 HashMap
来源：http://ezt.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://bah.ivvv.top

Ruby: // 手写 Hash
来源：http://kmd.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://sjo.fzhhl.top

[N08] 生成全排列
来源：http://wfb.havefunace.top

Py:   itertools.permutations(arr)
来源：http://buv.hesvh.cn

PHP:  // 手写递归交换
来源：http://yib.ctjpmb.com

JS:   // 手写回溯递归
来源：http://jrv.nwbrower.top

TS:   // 手写回溯递归
来源：http://xzy.dashuyun.cn

Java: // 手写回溯递归
来源：http://nil.epnwcf.com

Go:   // 手写回溯递归
来源：http://hee.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://dub.smart0.xyz

C#:   // 手写回溯递归
来源：http://dsg.yonumen.top

[N09] 栈与队列
来源：http://egn.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cws.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hep.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ait.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ujp.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hnd.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jfp.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cub.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cab.yuxming.cn

[N10] 链表节点定义
来源：http://ugx.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hyq.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yub.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pvj.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rpc.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://fev.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vfz.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zls.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vbh.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://ktc.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xid.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://kwi.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxt.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sro.gogol.net.cn

Java: // 手写递归
来源：http://axb.xuanzx.com

Go:   // 手写递归
来源：http://nck.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://crg.9152youxi.cn

C#:   // 手写递归
来源：http://mkl.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://inl.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://efa.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://myf.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cku.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tio.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fgq.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ujd.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://acb.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qcn.9152youxi.cn


<!-- 参考信息 -->