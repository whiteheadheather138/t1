代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dzo.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://twe.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vxm.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vyf.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rnf.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pwt.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vmv.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olg.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://osy.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hll.yj20258888.top

[K04] 读取 JSON 文件
来源：http://jxw.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ept.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zsp.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ybu.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://klx.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kxp.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jpu.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zjt.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bdv.daxiang520.top

[K05] 深拷贝对象
来源：http://vew.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://ina.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://zdt.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://bcr.tian-w.cn

TS:   structuredClone(obj)
来源：http://kwj.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://cai.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iyb.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gdi.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cup.yanxiufei.cn

[K06] 解析 URL 查询串
来源：http://egv.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iev.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nyl.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ais.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjy.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sej.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pfa.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ljo.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vkn.zhijiandao.cn

[K07] 进制转换
来源：http://ujd.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://akp.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hcg.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ytl.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vcn.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxq.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uom.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kln.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://idy.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://vxx.yj20258.top

Py:   pickle.dumps(obj)
来源：http://eyn.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kpp.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://orb.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bum.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://beo.316326.xyz

Go:   encoding/gob
来源：http://qux.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://ons.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hyl.tanke756.top

================================================================================
来源：http://rvx.sxryk.cn

L. 网络请求
来源：http://snp.dashuyun.cn

================================================================================
来源：http://ses.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://cjh.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cjz.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lmh.sxryk.cn

JS:   await fetch(url)
来源：http://ywc.nwbrower.top

TS:   await fetch(url)
来源：http://txx.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pkj.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://mgx.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zwy.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fls.zycfv.cn

[L02] 发送 POST JSON
来源：http://zil.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rmi.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ibt.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpw.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://phc.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mug.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kgf.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xoa.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rjo.shzxlz.cn

[L03] 设置自定义请求头
来源：http://ixg.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oeb.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bav.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gir.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqx.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ilu.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifc.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ksc.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kxl.cashguo.top

[L04] 设置超时
来源：http://xvd.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://exq.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvq.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vmw.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yut.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pkp.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivq.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gwz.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bys.yonumen.top

[L05] 上传文件（multipart）
来源：http://pkl.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qmp.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dav.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tyw.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rsu.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://htw.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dxa.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://snh.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xhj.yfazqb.com

[L06] 解析响应为 JSON
来源：http://qtp.hongshengwenyu.top

Py:   resp.json()
来源：http://yfr.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://het.chenzaomai.com

JS:   await resp.json()
来源：http://vpq.bjfxy.top

TS:   await resp.json()
来源：http://ywv.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vba.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xcm.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://tti.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hil.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://jnn.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gti.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oxe.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://tkx.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://ugp.cheryme.top

Java: resp.statusCode()
来源：http://qgh.yfazqb.com

Go:   resp.StatusCode
来源：http://zdo.316326.xyz

Ruby: resp.code.to_i
来源：http://bpm.yj20258.top

C#:   (int)resp.StatusCode
来源：http://cia.iojbl.cn

[L08] 并发请求多个地址
来源：http://iol.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ogo.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://hfd.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uem.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bqw.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ndt.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kmx.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vmz.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jom.uphjek.com

================================================================================
来源：http://aux.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://imp.haohaochexian.top

================================================================================
来源：http://anp.yueranfly.top

[M01] 读取命令行参数
来源：http://cdm.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://kjz.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://mgv.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://vyb.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://bmz.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://kpl.zycfv.cn

Go:   os.Args[1:]
来源：http://oxh.jqgufenzy.top

Ruby: ARGV
来源：http://lps.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://iio.xuetiantiany.cn

[M02] 读取环境变量
来源：http://nzb.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://fwz.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qqy.pengpengdd.cyou

JS:   process.env.HOME
来源：http://zay.xziqi.cn

TS:   process.env.HOME
来源：http://imx.haohaochexian.top

Java: System.getenv("HOME")
来源：http://yby.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lmh.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://bjn.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://trf.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://vks.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://auf.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bud.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vkl.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xqv.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://unp.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aoc.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://exf.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://snp.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://ekq.hesvh.cn

Py:   os.getcwd()
来源：http://cqq.ydzc1.top

PHP:  getcwd();
来源：http://gry.bbcook.cn

JS:   process.cwd()
来源：http://mbo.yanxiufei.cn

TS:   process.cwd()
来源：http://sxr.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://ypr.feifeiyinyue.top

Go:   os.Getwd()
来源：http://ccm.dashuyun.cn

Ruby: Dir.pwd
来源：http://rmb.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xdq.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://vfl.guannengcc.top

Py:   sys.exit(1)
来源：http://dwk.chenjidiqi.icu

PHP:  exit(1);
来源：http://ssa.fzhhl.top

JS:   process.exit(1)
来源：http://tra.redwolf501.top

TS:   process.exit(1)
来源：http://qgw.tian-w.cn

Java: System.exit(1)
来源：http://sox.shuidangran.top

Go:   os.Exit(1)
来源：http://tqb.c1oappe.top

Ruby: exit 1
来源：http://zyx.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zud.0kj1m.cn

[M06] 向标准错误输出
来源：http://ndg.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://tdz.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qtj.quarkkingdee.top

JS:   console.error("err")
来源：http://hvu.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://hch.aizwys.cn

Java: System.err.println("err")
来源：http://bka.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ukg.jqgufenzy.top

Ruby: warn "err"
来源：http://pvk.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://kpv.epnwcf.com

[M07] 判断是否为主入口
来源：http://jzb.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://hrj.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbz.zhixingplan.top

JS:   require.main === module
来源：http://wxp.jinyuanbaomall.cn

TS:   require.main === module
来源：http://zix.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://ort.dianchejie.cn

Go:   func main()
来源：http://lbw.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bwl.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://rdx.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://nee.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://zll.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://zmt.uphjek.com

JS:   process.platform;  process.version
来源：http://wwv.yj20258.top

TS:   process.platform;  process.version
来源：http://mla.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sot.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjr.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hoa.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hgi.uphjek.com

================================================================================
来源：http://vmg.9152youxi.cn

N. 数据结构与算法
来源：http://dhb.yangfankeji.com

================================================================================
来源：http://nvp.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://ref.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cip.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nqe.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmw.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sff.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://kye.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://eje.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gnj.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mcl.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://rko.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://say.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gmr.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mzn.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://cgb.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fbq.cheryme.top

Go:   slices.Sort(arr)
来源：http://zfg.fehbvm.com

Ruby: arr.sort
来源：http://lam.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kew.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://pjd.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dzj.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://piw.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gve.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qoj.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kba.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qno.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qii.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://rbm.c1oappe.top

[N04] 斐波那契数列
来源：http://koe.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://khb.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nqk.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yiu.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rot.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rjk.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kbo.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xit.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fms.jianghu66.top

[N05] 最大公约数
来源：http://nch.zycfv.cn

Py:   math.gcd(a, b)
来源：http://svt.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://piu.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kib.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zfh.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ttv.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qnk.guowangkeji.top

Ruby: a.gcd(b)
来源：http://chn.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://srb.ivvv.top

[N06] 判断回文字符串
来源：http://pjh.jlsjyb.cn

Py:   s == s[::-1]
来源：http://zgh.bbcook.cn

PHP:  $s === strrev($s);
来源：http://smy.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://ptt.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://mwi.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vih.c1oappe.top

Go:   // 双指针从两端比较
来源：http://xoj.shzxlz.cn

Ruby: s == s.reverse
来源：http://rpj.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uyf.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://moh.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://prs.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vzj.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nub.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://sgo.gzhubu.top

Java: // 手写 HashMap
来源：http://ndr.hcnkem.com

Go:   // 手写 map[int]int
来源：http://dli.sufxvd.cn

Ruby: // 手写 Hash
来源：http://jmc.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iuk.bjfxy.top

[N08] 生成全排列
来源：http://dji.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://php.xylfe.cn

PHP:  // 手写递归交换
来源：http://rou.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://hko.tanke756.top

TS:   // 手写回溯递归
来源：http://eom.sufxvd.cn

Java: // 手写回溯递归
来源：http://zkb.zycfv.cn

Go:   // 手写回溯递归
来源：http://wti.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://mhq.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://zzg.svipenyu.cn

[N09] 栈与队列
来源：http://loy.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jqz.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nov.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rds.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://raj.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://frp.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vny.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cpt.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ikf.zhengqikj.top

[N10] 链表节点定义
来源：http://wvv.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sys.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tlq.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gry.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apu.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://ewf.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://rpa.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nzr.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xwh.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://lei.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sjo.yangfankeji.com


<!-- 参考信息 -->