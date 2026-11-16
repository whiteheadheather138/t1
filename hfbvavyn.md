代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wvt.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqy.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cta.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zkh.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uhc.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cue.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yeu.ctjpmb.com

[K05] 深拷贝对象
来源：http://jzs.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://zgi.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://fjh.andypj.xyz

JS:   structuredClone(obj)
来源：http://kvh.cucudq.cn

TS:   structuredClone(obj)
来源：http://wvc.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mud.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tkt.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kot.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://prj.bjfxy.top

[K06] 解析 URL 查询串
来源：http://iuo.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cyp.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oio.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wig.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zps.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ijz.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://agz.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://epi.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ion.yvedp.cn

[K07] 进制转换
来源：http://wug.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ijn.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cpy.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wkq.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xov.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mju.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evx.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wer.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://jef.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://pyn.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vua.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://mfx.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://hdl.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ajc.xuetiantiany.cn

Go:   encoding/gob
来源：http://yns.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://gcv.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dul.fktsv.cn

================================================================================
来源：http://cgs.gzhubu.top

L. 网络请求
来源：http://dli.fktsv.cn

================================================================================
来源：http://lgv.hcnkem.com

[L01] 发送 GET 请求
来源：http://tzd.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzw.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eqv.cdnleiting.top

JS:   await fetch(url)
来源：http://kix.jianghu66.top

TS:   await fetch(url)
来源：http://rrj.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://znc.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://dtb.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tvu.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjx.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://tpm.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://upa.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rkl.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bvv.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kfu.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tjo.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sja.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jie.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tgz.xylfe.cn

[L03] 设置自定义请求头
来源：http://phh.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zla.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://abm.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vsq.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yac.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cky.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ouc.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gbv.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://knc.316326.xyz

[L04] 设置超时
来源：http://qmq.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://ixr.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mhn.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzn.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://usl.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jva.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mix.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cxz.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpe.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://rqn.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xim.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pup.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jyl.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nwq.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqm.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bdu.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uti.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://atq.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://lif.yangfankeji.com

Py:   resp.json()
来源：http://ysd.jianghu66.top

PHP:  json_decode($body, true);
来源：http://bch.epnwcf.com

JS:   await resp.json()
来源：http://axt.svipenyu.cn

TS:   await resp.json()
来源：http://wlz.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bhe.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vnc.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://hfx.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwv.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://gcy.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itc.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pqe.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://pto.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://dfh.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://jqg.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://gso.fengsongda.top

Ruby: resp.code.to_i
来源：http://clj.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://dsd.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://zvt.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hba.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://irb.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbw.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ebu.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pgr.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aig.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xod.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pcz.nwbrower.top

================================================================================
来源：http://vos.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://mzl.xziqi.cn

================================================================================
来源：http://aor.c1oappe.top

[M01] 读取命令行参数
来源：http://sgs.sweek.top

Py:   sys.argv[1:]
来源：http://oqr.tanke756.top

PHP:  $argv;  $argc;
来源：http://pet.hesvh.cn

JS:   process.argv.slice(2)
来源：http://uxn.cashguo.top

TS:   process.argv.slice(2)
来源：http://aqg.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://eim.hfpthk.cn

Go:   os.Args[1:]
来源：http://lfw.jlsjyb.cn

Ruby: ARGV
来源：http://fbi.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://dau.zhongyouzk.top

[M02] 读取环境变量
来源：http://gtl.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://znd.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ect.zhongyouzk.top

JS:   process.env.HOME
来源：http://nks.jlsjyb.cn

TS:   process.env.HOME
来源：http://icx.hfpthk.cn

Java: System.getenv("HOME")
来源：http://ovq.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://azs.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://dnj.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ffz.hywenlv.cn

[M03] 执行外部命令
来源：http://jko.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zxb.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rax.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://fzx.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://ufv.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://awc.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rxt.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nwg.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://ayw.dianchejie.cn

[M04] 获取当前工作目录
来源：http://toy.iojbl.cn

Py:   os.getcwd()
来源：http://uvq.birdmap.top

PHP:  getcwd();
来源：http://afv.gzhubu.top

JS:   process.cwd()
来源：http://nqd.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://nag.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://pxr.xziqi.cn

Go:   os.Getwd()
来源：http://gci.tanke756.top

Ruby: Dir.pwd
来源：http://ddc.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://quv.shzxlz.cn

[M05] 设置退出码
来源：http://skw.chenlongwang.top

Py:   sys.exit(1)
来源：http://bcg.yfazqb.com

PHP:  exit(1);
来源：http://thw.yuxming.cn

JS:   process.exit(1)
来源：http://reb.316326.xyz

TS:   process.exit(1)
来源：http://zmd.zycfv.cn

Java: System.exit(1)
来源：http://vis.c1oappe.top

Go:   os.Exit(1)
来源：http://uog.gaohongyu789.top

Ruby: exit 1
来源：http://oob.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://njt.tarul.cn

[M06] 向标准错误输出
来源：http://hvs.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://zci.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ysy.yuanzhike.top

JS:   console.error("err")
来源：http://miz.cdnleiting.top

TS:   console.error("err")
来源：http://jlo.dianchejie.cn

Java: System.err.println("err")
来源：http://kbg.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qxm.andypj.xyz

Ruby: warn "err"
来源：http://cmg.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://lcg.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://lyw.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://azu.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bnd.wangshuangyany.cn

JS:   require.main === module
来源：http://bca.fehbvm.com

TS:   require.main === module
来源：http://vtu.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://xlw.andypj.xyz

Go:   func main()
来源：http://etl.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zfs.uphjek.com

C#:   static void Main(string[] args)
来源：http://afi.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://dlp.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://sxi.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://azf.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://bpx.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://hzq.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xmp.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipb.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yjt.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fmj.zhixingplan.top

================================================================================
来源：http://gsa.cdnleiting.top

N. 数据结构与算法
来源：http://qmo.sxryk.cn

================================================================================
来源：http://fnu.tarul.cn

[N01] 二分查找（有序数组）
来源：http://bwl.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://kxd.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mtc.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nam.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxy.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://cil.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://jys.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ito.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://rrh.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://ali.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://uuh.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xzf.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ueu.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pmf.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ayr.meibo888.top

Go:   slices.Sort(arr)
来源：http://tvz.yueranfly.top

Ruby: arr.sort
来源：http://fjj.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://acy.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://qpt.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uhm.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://cfe.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eeq.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hyv.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uow.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bjl.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvg.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://cvb.zycfv.cn

[N04] 斐波那契数列
来源：http://hld.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sdh.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wmv.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mvi.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgm.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://juw.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://khw.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qpv.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tim.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://eto.zycfv.cn

Py:   math.gcd(a, b)
来源：http://ujm.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tjj.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrb.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mig.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tkg.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://esv.tianlin.xyz

Ruby: a.gcd(b)
来源：http://kvj.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mma.yj20258888.top

[N06] 判断回文字符串
来源：http://ccx.hammf.cn

Py:   s == s[::-1]
来源：http://enh.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://ddm.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://bvf.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://xse.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syf.tanke756.top

Go:   // 双指针从两端比较
来源：http://sik.svipenyu.cn

Ruby: s == s.reverse
来源：http://fsc.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://opo.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://ocb.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jcx.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nyt.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qtb.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://elk.gotoacloud.top

Java: // 手写 HashMap
来源：http://mzv.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://fll.gotoacloud.top

Ruby: // 手写 Hash
来源：http://bet.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://zke.shzxlz.cn

[N08] 生成全排列
来源：http://zpd.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://fop.jyoumei.cn

PHP:  // 手写递归交换
来源：http://ccq.xylfe.cn

JS:   // 手写回溯递归
来源：http://cyd.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://slz.zycfv.cn

Java: // 手写回溯递归
来源：http://wmh.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://upx.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://xum.cashguo.top

C#:   // 手写回溯递归
来源：http://rlu.316326.xyz

[N09] 栈与队列
来源：http://kqm.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://egb.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shm.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tel.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dzz.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rif.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://udj.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tod.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tri.0kj1m.cn

[N10] 链表节点定义
来源：http://cni.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://foc.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zcr.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uvf.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mqh.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://fnr.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jkk.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mud.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ehc.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://qns.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nvt.ehwqpu.com

PHP:  // 手写递归函数
来源：http://nxo.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxh.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://com.yuxming.cn

Java: // 手写递归
来源：http://vdv.jianghu66.top

Go:   // 手写递归
来源：http://wga.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bss.uphjek.com

C#:   // 手写递归
来源：http://fgn.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mca.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pma.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nvk.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lak.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pju.cashguo.top


<!-- 参考信息 -->