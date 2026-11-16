代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tig.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hyd.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrp.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zjm.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eeq.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://oyg.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://krv.fehbvm.com

[K05] 深拷贝对象
来源：http://qio.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://ren.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://gla.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://nig.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://vdh.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oym.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yfm.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://swb.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://qkb.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://nfj.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cov.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bgt.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nkw.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytk.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://knx.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://qgw.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zuc.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lgx.quarkkingdee.top

[K07] 进制转换
来源：http://eba.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ulk.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ksl.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://riq.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rbh.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dyy.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://img.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qoq.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iuo.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://yor.pycfn.com

Py:   pickle.dumps(obj)
来源：http://yjb.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pev.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://qpv.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://srn.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mno.wangdashe.top

Go:   encoding/gob
来源：http://lrx.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://alc.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afx.yj20258.top

================================================================================
来源：http://nym.havefunace.top

L. 网络请求
来源：http://sxb.ydjk.org.cn

================================================================================
来源：http://ebg.fzhhl.top

[L01] 发送 GET 请求
来源：http://gut.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gtr.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://owe.chenzaomai.com

JS:   await fetch(url)
来源：http://vvq.yuanzhike.top

TS:   await fetch(url)
来源：http://jjn.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rds.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://ucd.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bjs.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://adn.meibo888.top

[L02] 发送 POST JSON
来源：http://yhx.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pvp.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pyj.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpk.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wah.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jlu.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pef.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mjk.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aos.yueranfly.top

[L03] 设置自定义请求头
来源：http://inv.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eoy.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nhv.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsw.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjf.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ttg.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fhr.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yjp.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wjp.cucudq.cn

[L04] 设置超时
来源：http://tnm.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://tvg.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zyw.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ftr.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxr.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bfz.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pkp.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://roe.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txt.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://kzz.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vun.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oij.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ryl.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bgp.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://djq.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzn.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hhv.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uqt.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://snx.cucudq.cn

Py:   resp.json()
来源：http://avo.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://ogr.jqgfzy.top

JS:   await resp.json()
来源：http://vza.shanyushiyangtech.top

TS:   await resp.json()
来源：http://kcu.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cpr.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pjt.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://jye.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mng.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://rjy.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://znm.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nkl.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://wwb.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://col.52xcode.cn

Java: resp.statusCode()
来源：http://ilr.zhoulong.xyz

Go:   resp.StatusCode
来源：http://duy.yfazqb.com

Ruby: resp.code.to_i
来源：http://xbe.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://ecf.chenzaomai.com

[L08] 并发请求多个地址
来源：http://ntu.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gey.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://asd.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wpw.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yri.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bvo.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vpr.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fhg.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fyb.iojbl.cn

================================================================================
来源：http://udv.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://aro.jqgfzy.top

================================================================================
来源：http://cbh.dianchejie.cn

[M01] 读取命令行参数
来源：http://bec.daria6918.cn

Py:   sys.argv[1:]
来源：http://esk.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://har.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://cdv.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://czp.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://jal.hesvh.cn

Go:   os.Args[1:]
来源：http://icx.sufxvd.cn

Ruby: ARGV
来源：http://dxe.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://ttj.cheryme.top

[M02] 读取环境变量
来源：http://cns.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://npx.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vnw.fktsv.cn

JS:   process.env.HOME
来源：http://hgn.snrcjt.cn

TS:   process.env.HOME
来源：http://krc.meibo888.top

Java: System.getenv("HOME")
来源：http://luf.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bpp.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://pvu.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nki.tanke756.top

[M03] 执行外部命令
来源：http://sgt.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cvg.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://seo.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uil.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://msr.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nmt.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mnk.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vqo.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://inh.jianghu66.top

[M04] 获取当前工作目录
来源：http://gbj.yueranfly.top

Py:   os.getcwd()
来源：http://rcz.gogol.net.cn

PHP:  getcwd();
来源：http://egc.shangyingyoupin.top

JS:   process.cwd()
来源：http://sey.chenlongwang.top

TS:   process.cwd()
来源：http://owv.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://qtw.yongpay.top

Go:   os.Getwd()
来源：http://lbh.shzxlz.cn

Ruby: Dir.pwd
来源：http://qfk.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://qgy.cucudq.cn

[M05] 设置退出码
来源：http://hcu.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://jop.tian-w.cn

PHP:  exit(1);
来源：http://oik.yanxiufei.cn

JS:   process.exit(1)
来源：http://iuc.andypj.xyz

TS:   process.exit(1)
来源：http://qpb.bbcook.cn

Java: System.exit(1)
来源：http://vxj.xziqi.cn

Go:   os.Exit(1)
来源：http://qmi.zhongyouzk.top

Ruby: exit 1
来源：http://tdt.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qbr.shzxlz.cn

[M06] 向标准错误输出
来源：http://jho.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://hru.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wzb.hnxiangtu.top

JS:   console.error("err")
来源：http://fct.aibaodan.cn

TS:   console.error("err")
来源：http://xwk.zhiwuduotai.top

Java: System.err.println("err")
来源：http://uxm.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jhx.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://nya.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://xtj.9152youxi.cn

[M07] 判断是否为主入口
来源：http://epm.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://lqk.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dsu.yangfankeji.com

JS:   require.main === module
来源：http://njt.uphjek.com

TS:   require.main === module
来源：http://xuk.nanxinkj.top

Java: public static void main(String[] args)
来源：http://dne.shangyingyoupin.top

Go:   func main()
来源：http://zgm.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ulj.daxiang520.top

C#:   static void Main(string[] args)
来源：http://ssk.hammf.cn

[M08] 获取系统与运行时信息
来源：http://tef.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://uqh.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://mju.tanke756.top

JS:   process.platform;  process.version
来源：http://jjb.yvedp.cn

TS:   process.platform;  process.version
来源：http://aws.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nww.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://cch.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://roo.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wlt.wangshuangyany.cn

================================================================================
来源：http://skb.zhongyouzk.top

N. 数据结构与算法
来源：http://ept.iojbl.cn

================================================================================
来源：http://mhz.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://vim.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://hpx.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jzw.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bre.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nhw.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://xry.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://yuc.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tdn.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://vqr.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://aci.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://qas.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckc.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vao.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wih.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zev.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://hti.shangyingyoupin.top

Ruby: arr.sort
来源：http://fzd.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zka.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://xpz.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://egs.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://gum.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vya.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vhy.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://abr.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cig.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xbj.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://nmn.yj20258.top

[N04] 斐波那契数列
来源：http://zfd.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xeq.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwm.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zbe.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wub.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ncb.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pjp.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sje.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gnf.cucudq.cn

[N05] 最大公约数
来源：http://lms.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://aga.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rzk.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pxb.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrv.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nby.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ein.tarul.cn

Ruby: a.gcd(b)
来源：http://lnj.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tnb.cdnleiting.top

[N06] 判断回文字符串
来源：http://kzi.jqgufenzy.top

Py:   s == s[::-1]
来源：http://zgd.hesvh.cn

PHP:  $s === strrev($s);
来源：http://kgc.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://fvc.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://jwe.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mse.mhx1999.top

Go:   // 双指针从两端比较
来源：http://vdu.sufxvd.cn

Ruby: s == s.reverse
来源：http://kqo.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lkn.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://wfg.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uip.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ugx.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gww.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://bwd.ybcxt.top

Java: // 手写 HashMap
来源：http://tqi.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://amy.aizwys.cn

Ruby: // 手写 Hash
来源：http://abp.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ivi.wangdashe.top

[N08] 生成全排列
来源：http://ydv.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://osh.yj20258.top

PHP:  // 手写递归交换
来源：http://jhc.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://yhz.shuidangran.top

TS:   // 手写回溯递归
来源：http://fbv.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://hkb.yonumen.top

Go:   // 手写回溯递归
来源：http://xco.yj20258.top

Ruby: arr.permutation.to_a
来源：http://ssb.yongpay.top

C#:   // 手写回溯递归
来源：http://bax.hysaishi.cn

[N09] 栈与队列
来源：http://gre.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bkv.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nbc.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ami.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://anb.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fiw.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dpi.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wns.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lkg.shuidangran.top

[N10] 链表节点定义
来源：http://kpc.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://amo.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://moi.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://owp.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fyo.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://tmb.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://gof.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://enr.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kfs.vehdjk.com

[N11] 二叉树中序遍历
来源：http://mwk.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://son.jianghu66.top

PHP:  // 手写递归函数
来源：http://xrd.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dmh.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cen.pengpengdd.cyou

Java: // 手写递归
来源：http://onz.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://rqi.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xiz.gaohongyu789.top

C#:   // 手写递归
来源：http://zxz.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xcj.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fjd.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fwc.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szr.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oro.jianghu66.top


<!-- 参考信息 -->