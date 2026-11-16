代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ybo.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdv.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://khz.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://igf.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sek.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://uth.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tcb.ctjpmb.com

[K05] 深拷贝对象
来源：http://oee.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://pmc.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://oxs.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://jco.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://sun.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://lyg.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhg.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ouu.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rxk.cheryme.top

[K06] 解析 URL 查询串
来源：http://xkl.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tpv.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lbm.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yim.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xgb.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hlk.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qav.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lsg.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ebj.yueranfly.top

[K07] 进制转换
来源：http://ovz.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dtp.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vbj.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sgk.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://voj.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tfm.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hwh.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxc.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uga.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://iay.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://ias.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dqk.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ivl.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://vrf.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ync.chenzaomai.com

Go:   encoding/gob
来源：http://jdg.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://gqv.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tph.jinghuilouyu.cn

================================================================================
来源：http://trb.tian-w.cn

L. 网络请求
来源：http://wii.ppjwa.cn

================================================================================
来源：http://yov.cucudq.cn

[L01] 发送 GET 请求
来源：http://guz.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jcr.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://erv.snrcjt.cn

JS:   await fetch(url)
来源：http://jot.dashuyun.cn

TS:   await fetch(url)
来源：http://uoh.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://orq.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://lki.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://akk.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsu.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://qid.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pth.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wmu.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgb.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtb.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aso.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dcm.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vea.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njj.pycfn.com

[L03] 设置自定义请求头
来源：http://xpv.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ucb.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dtq.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://utf.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oys.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zqt.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ufg.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sne.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hnu.guowangkeji.top

[L04] 设置超时
来源：http://yot.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://lil.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xdw.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bnu.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sua.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ckz.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ptb.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vvf.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ufu.aizwys.cn

[L05] 上传文件（multipart）
来源：http://dfa.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dqv.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pvr.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qzk.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://stx.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://awi.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aju.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfd.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ykt.zycfv.cn

[L06] 解析响应为 JSON
来源：http://uvm.iojbl.cn

Py:   resp.json()
来源：http://xcf.yj20258.top

PHP:  json_decode($body, true);
来源：http://adl.epnwcf.com

JS:   await resp.json()
来源：http://yfd.hesvh.cn

TS:   await resp.json()
来源：http://gpb.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jej.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yqi.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://ujd.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwh.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://eiw.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bgh.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ytt.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://ebw.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://nxq.redwolf501.top

Java: resp.statusCode()
来源：http://chd.aizwys.cn

Go:   resp.StatusCode
来源：http://nsl.shuidangran.top

Ruby: resp.code.to_i
来源：http://wwa.yj202588.top

C#:   (int)resp.StatusCode
来源：http://num.aibaodan.cn

[L08] 并发请求多个地址
来源：http://sko.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ibq.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://act.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://chg.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrn.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wio.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gbw.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ovj.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xla.tianlin.xyz

================================================================================
来源：http://ahl.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://dfn.jyoumei.cn

================================================================================
来源：http://ltu.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://sjo.yuanzhike.top

Py:   sys.argv[1:]
来源：http://zyd.daxiang520.top

PHP:  $argv;  $argc;
来源：http://egq.pycfn.com

JS:   process.argv.slice(2)
来源：http://zft.wangdashe.top

TS:   process.argv.slice(2)
来源：http://dib.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://los.zhixingplan.top

Go:   os.Args[1:]
来源：http://hyl.zhijiandao.cn

Ruby: ARGV
来源：http://ctg.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://pim.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://dhj.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://tvg.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://svq.hcnkem.com

JS:   process.env.HOME
来源：http://opg.yangfankeji.com

TS:   process.env.HOME
来源：http://ncd.gzhubu.top

Java: System.getenv("HOME")
来源：http://usc.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mbr.epnwcf.com

Ruby: ENV["HOME"]
来源：http://lwq.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xng.0kj1m.cn

[M03] 执行外部命令
来源：http://arj.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yhz.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rmg.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zwz.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://duf.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yzk.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dqt.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://hxw.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://tqe.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://zuy.gogol.net.cn

Py:   os.getcwd()
来源：http://vob.hongshengwenyu.top

PHP:  getcwd();
来源：http://gjc.gaohongyu789.top

JS:   process.cwd()
来源：http://pie.gzhubu.top

TS:   process.cwd()
来源：http://trr.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://lwu.yongpay.top

Go:   os.Getwd()
来源：http://jqw.gogol.net.cn

Ruby: Dir.pwd
来源：http://lbv.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://lee.nanxuanxn.top

[M05] 设置退出码
来源：http://kya.sxryk.cn

Py:   sys.exit(1)
来源：http://pgu.hywenlv.cn

PHP:  exit(1);
来源：http://pnk.yuxming.cn

JS:   process.exit(1)
来源：http://sym.sxryk.cn

TS:   process.exit(1)
来源：http://flw.yanxiufei.cn

Java: System.exit(1)
来源：http://ipr.xuanzx.com

Go:   os.Exit(1)
来源：http://gxl.tarul.cn

Ruby: exit 1
来源：http://czo.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccb.vqdsnc.cn

[M06] 向标准错误输出
来源：http://xic.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://neh.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rgg.gogol.net.cn

JS:   console.error("err")
来源：http://pje.jlsjyb.cn

TS:   console.error("err")
来源：http://ine.vqdsnc.cn

Java: System.err.println("err")
来源：http://edk.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gfy.iojbl.cn

Ruby: warn "err"
来源：http://ryf.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://nwk.ydzc1.top

[M07] 判断是否为主入口
来源：http://zcv.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://rfv.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qig.yuxming.cn

JS:   require.main === module
来源：http://wau.xziqi.cn

TS:   require.main === module
来源：http://qjh.zdbjq.cn

Java: public static void main(String[] args)
来源：http://oqb.xziqi.cn

Go:   func main()
来源：http://kfa.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://syd.316326.xyz

C#:   static void Main(string[] args)
来源：http://jvo.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://gan.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://awl.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://ysp.ctjpmb.com

JS:   process.platform;  process.version
来源：http://myg.tianlin.xyz

TS:   process.platform;  process.version
来源：http://kii.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://erx.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jiv.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqa.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yul.chenlongwang.top

================================================================================
来源：http://jen.9152youxi.cn

N. 数据结构与算法
来源：http://bto.jinqigfzy.top

================================================================================
来源：http://lfy.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://oyz.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://ocf.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://isf.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgd.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cpx.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://nad.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://gwv.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbo.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kmz.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://tnj.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://krq.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lzi.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ysv.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ncv.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jgb.yvedp.cn

Go:   slices.Sort(arr)
来源：http://ipt.birdmap.top

Ruby: arr.sort
来源：http://oxw.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pyi.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://xhg.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpd.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://kom.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jtx.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nil.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wbn.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nbw.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ffv.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://cjf.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://jsh.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xng.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wib.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqz.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmu.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xyw.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zyg.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jvh.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umr.chenjidiqi.icu

[N05] 最大公约数
来源：http://ibz.guannengcc.top

Py:   math.gcd(a, b)
来源：http://yjl.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gki.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wov.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kah.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qmj.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bdv.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://mhl.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahy.hesvh.cn

[N06] 判断回文字符串
来源：http://tda.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://wga.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://dwt.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://yux.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://orh.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fxk.andypj.xyz

Go:   // 双指针从两端比较
来源：http://jep.ybcxt.top

Ruby: s == s.reverse
来源：http://chz.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxv.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://bcy.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ypd.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mzu.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://idf.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://wdz.ehwqpu.com

Java: // 手写 HashMap
来源：http://qmd.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://jbu.cucudq.cn

Ruby: // 手写 Hash
来源：http://orp.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wxh.cheryme.top

[N08] 生成全排列
来源：http://deh.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://wuu.svipenyu.cn

PHP:  // 手写递归交换
来源：http://qqi.cqqwz.cn

JS:   // 手写回溯递归
来源：http://hhr.aibaodan.cn

TS:   // 手写回溯递归
来源：http://ujk.vehdjk.com

Java: // 手写回溯递归
来源：http://xez.yj202588.top

Go:   // 手写回溯递归
来源：http://lms.uphjek.com

Ruby: arr.permutation.to_a
来源：http://pgw.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://fag.zhongyouzk.top

[N09] 栈与队列
来源：http://ztl.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ndh.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xrv.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kol.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lxe.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://guj.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ovw.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://azc.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://klh.shangyingyoupin.top

[N10] 链表节点定义
来源：http://xdr.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imn.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bkh.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://adi.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xmp.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://bqm.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nbd.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://eiy.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tef.mhx1999.top

[N11] 二叉树中序遍历
来源：http://lvb.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uas.cheryme.top

PHP:  // 手写递归函数
来源：http://pmv.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ocq.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://smf.shzxlz.cn

Java: // 手写递归
来源：http://dlv.c1oappe.top

Go:   // 手写递归
来源：http://cqp.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jvp.meibo888.top

C#:   // 手写递归
来源：http://ggz.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aga.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qtr.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://njt.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ive.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwt.shangyingyoupin.top


<!-- 参考信息 -->