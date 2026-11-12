代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wgk.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pzb.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vlt.gogol.net.cn

[K05] 深拷贝对象
来源：http://mxr.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://tfs.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://znm.meibo888.top

JS:   structuredClone(obj)
来源：http://ndt.xylfe.cn

TS:   structuredClone(obj)
来源：http://nzx.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cdt.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qoe.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://whx.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ksc.hesvh.cn

[K06] 解析 URL 查询串
来源：http://laz.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myq.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfb.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rcs.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zun.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dvi.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dhn.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dfo.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mvb.yj20258.top

[K07] 进制转换
来源：http://xot.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cbc.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wbw.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bnl.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vmu.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fko.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gzw.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qwt.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dbi.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://jrf.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://qcx.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wtk.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://gge.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://zom.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ytp.ehwqpu.com

Go:   encoding/gob
来源：http://xtz.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://ple.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gdx.smart0.xyz

================================================================================
来源：http://vni.yongpay.top

L. 网络请求
来源：http://tgg.sxryk.cn

================================================================================
来源：http://mtj.52xcode.cn

[L01] 发送 GET 请求
来源：http://ziw.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tzz.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wms.cdnleiting.top

JS:   await fetch(url)
来源：http://wym.shangyingyoupin.top

TS:   await fetch(url)
来源：http://abj.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nhj.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://tqd.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vvm.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fhm.svipenyu.cn

[L02] 发送 POST JSON
来源：http://mqh.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://rkz.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uyd.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fgk.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyt.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://srd.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bkn.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ynf.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fsh.ybcxt.top

[L03] 设置自定义请求头
来源：http://top.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aog.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bar.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://alw.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zib.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xlu.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vlq.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tik.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ctl.shzxlz.cn

[L04] 设置超时
来源：http://myh.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://qhz.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rhv.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhc.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ocn.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vlm.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ssi.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nww.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ono.pycfn.com

[L05] 上传文件（multipart）
来源：http://ifp.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kzp.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pia.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cys.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xim.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://syt.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://clm.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vgi.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lbo.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://jyr.ctjpmb.com

Py:   resp.json()
来源：http://qyb.yj20258.top

PHP:  json_decode($body, true);
来源：http://ler.cdnleiting.top

JS:   await resp.json()
来源：http://jxu.9152youxi.cn

TS:   await resp.json()
来源：http://awm.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wzb.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xne.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://bio.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://did.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://aij.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://quj.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://syq.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://vhq.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://jph.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://wtw.sweek.top

Go:   resp.StatusCode
来源：http://eal.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://cxz.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://lsg.andypj.xyz

[L08] 并发请求多个地址
来源：http://tnt.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xwc.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://gxz.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryo.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfk.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xel.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dbk.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sed.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvt.yj202588.top

================================================================================
来源：http://dsa.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://nso.ydzc1.top

================================================================================
来源：http://dem.tanke756.top

[M01] 读取命令行参数
来源：http://cyg.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://dmn.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://ird.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://aoh.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://hab.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://giw.bbcook.cn

Go:   os.Args[1:]
来源：http://qij.daria6918.cn

Ruby: ARGV
来源：http://cnf.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://qma.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://pjb.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://xyr.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xeo.bbcook.cn

JS:   process.env.HOME
来源：http://xpd.zhoulong.xyz

TS:   process.env.HOME
来源：http://ytc.epnwcf.com

Java: System.getenv("HOME")
来源：http://tur.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dvj.bjfxy.top

Ruby: ENV["HOME"]
来源：http://bjy.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fxk.fzhhl.top

[M03] 执行外部命令
来源：http://bzp.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gdg.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tjp.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yyr.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://knw.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dgp.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wzp.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://gea.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://yuw.hfpthk.cn

[M04] 获取当前工作目录
来源：http://dnp.jinqigfzy.top

Py:   os.getcwd()
来源：http://egr.aibaodan.cn

PHP:  getcwd();
来源：http://ckt.fehbvm.com

JS:   process.cwd()
来源：http://wya.jinqigufen.top

TS:   process.cwd()
来源：http://ofn.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://uxn.fengsongda.top

Go:   os.Getwd()
来源：http://zdz.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://zqw.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://dau.ivvv.top

[M05] 设置退出码
来源：http://mrv.smart0.xyz

Py:   sys.exit(1)
来源：http://gao.hongshengwenyu.top

PHP:  exit(1);
来源：http://fge.cashguo.top

JS:   process.exit(1)
来源：http://zol.nwbrower.top

TS:   process.exit(1)
来源：http://usr.yongpay.top

Java: System.exit(1)
来源：http://kfz.ybcxt.top

Go:   os.Exit(1)
来源：http://xkw.hysaishi.cn

Ruby: exit 1
来源：http://yap.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eww.bbcook.cn

[M06] 向标准错误输出
来源：http://dxj.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://qni.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pse.52xcode.cn

JS:   console.error("err")
来源：http://nkk.yvedp.cn

TS:   console.error("err")
来源：http://yxh.wangshuangyany.cn

Java: System.err.println("err")
来源：http://kqb.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dmt.tanke756.top

Ruby: warn "err"
来源：http://bzu.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://xel.yuxming.cn

[M07] 判断是否为主入口
来源：http://quk.yj20258.top

Py:   if __name__ == "__main__":
来源：http://rwz.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fui.zdqjudy.top

JS:   require.main === module
来源：http://bgu.birdmap.top

TS:   require.main === module
来源：http://xex.yuxming.cn

Java: public static void main(String[] args)
来源：http://vcz.aibaodan.cn

Go:   func main()
来源：http://ztw.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://osh.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://ckm.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://jbt.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://zgf.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://fyr.zdqjudy.top

JS:   process.platform;  process.version
来源：http://atp.smart0.xyz

TS:   process.platform;  process.version
来源：http://nuo.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://adr.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ijn.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rqx.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kic.dianchejie.cn

================================================================================
来源：http://zmp.yj20258888.top

N. 数据结构与算法
来源：http://bho.gaohongyu789.top

================================================================================
来源：http://luk.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://puw.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://zrg.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ykj.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ukz.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqr.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ncc.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://nwd.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fnx.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://slu.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://ujn.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://jny.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckg.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wfx.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pxg.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvw.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://gzr.zhengqikj.top

Ruby: arr.sort
来源：http://mar.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qvs.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://yqn.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnd.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://oew.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnd.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cno.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://epw.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cua.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qst.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://lai.cucudq.cn

[N04] 斐波那契数列
来源：http://hgw.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ojs.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tbs.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fbg.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yui.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://whp.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zhv.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yqv.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ukw.tarul.cn

[N05] 最大公约数
来源：http://luk.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://ovu.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uwq.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzm.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfx.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://smu.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gaj.yongpay.top

Ruby: a.gcd(b)
来源：http://bnt.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cky.xziqi.cn

[N06] 判断回文字符串
来源：http://gcy.hysaishi.cn

Py:   s == s[::-1]
来源：http://qkn.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://eaa.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://jbd.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://azx.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zso.tarul.cn

Go:   // 双指针从两端比较
来源：http://sdf.yfazqb.com

Ruby: s == s.reverse
来源：http://qpm.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://psa.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://auj.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://smn.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ipr.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wqw.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://iov.gogol.net.cn

Java: // 手写 HashMap
来源：http://std.yuxming.cn

Go:   // 手写 map[int]int
来源：http://jzl.cheryme.top

Ruby: // 手写 Hash
来源：http://bub.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://pyq.epnwcf.com

[N08] 生成全排列
来源：http://tuw.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://dyt.fengsongda.top

PHP:  // 手写递归交换
来源：http://rvv.haohaochexian.top

JS:   // 手写回溯递归
来源：http://evy.jqgfzy.top

TS:   // 手写回溯递归
来源：http://hax.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://nnj.316326.xyz

Go:   // 手写回溯递归
来源：http://rof.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://akn.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://pfy.sxryk.cn

[N09] 栈与队列
来源：http://oqk.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://isj.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hux.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mjn.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jbb.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lim.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mxo.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwz.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zxe.hnqzz.top

[N10] 链表节点定义
来源：http://faj.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://avw.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eke.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kui.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hpp.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://oxt.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://jsg.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://krz.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cvl.ydzc1.top

[N11] 二叉树中序遍历
来源：http://ocv.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lpw.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://ewo.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikb.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vgm.jianghu66.top

Java: // 手写递归
来源：http://qpl.tarul.cn

Go:   // 手写递归
来源：http://odt.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tqj.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://tsb.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncc.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lil.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://plt.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tmn.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bep.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://upc.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gem.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rqw.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://amv.aizwys.cn


<!-- 参考信息 -->