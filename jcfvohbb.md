代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://igd.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://ywc.tian-w.cn

JS:   structuredClone(obj)
来源：http://civ.aibaodan.cn

TS:   structuredClone(obj)
来源：http://ebt.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hyr.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://crz.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://roh.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vaj.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://imq.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wfi.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pgl.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvp.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfp.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xna.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ehv.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uia.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kur.hfpthk.cn

[K07] 进制转换
来源：http://dum.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://chf.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cwt.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjx.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hdi.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pgx.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jus.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mzo.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xpp.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://sfy.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://paa.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pox.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://xiq.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://kma.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hyz.sysykeji.top

Go:   encoding/gob
来源：http://hac.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://arc.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vat.jinghuilouyu.cn

================================================================================
来源：http://xtx.zhiwuduotai.top

L. 网络请求
来源：http://zvv.yonumen.top

================================================================================
来源：http://zkd.xinyue.icu

[L01] 发送 GET 请求
来源：http://eyx.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ilw.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xqn.sxryk.cn

JS:   await fetch(url)
来源：http://uxi.yj202588.top

TS:   await fetch(url)
来源：http://kzt.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nua.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://wmd.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lrh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ist.nanxinkj.top

[L02] 发送 POST JSON
来源：http://qct.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://qdd.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iun.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lie.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsu.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hgq.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hnr.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aqr.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yfk.yuanzhike.top

[L03] 设置自定义请求头
来源：http://zel.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yrd.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qnr.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sjs.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfh.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mab.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jym.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://viy.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gvk.xylfe.cn

[L04] 设置超时
来源：http://nne.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://qic.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sdf.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pqt.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gmk.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xkk.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xph.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fdj.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lwj.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://xfi.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wpz.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rzy.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zdb.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zqg.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fkh.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cfr.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fth.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vvr.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://qmy.yj20258.top

Py:   resp.json()
来源：http://deh.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://aje.vehdjk.com

JS:   await resp.json()
来源：http://dmr.sjlbkw.cn

TS:   await resp.json()
来源：http://cky.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eet.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://trq.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://eac.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scw.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://qdi.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tkq.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ixs.ivvv.top

JS:   resp.ok;  resp.status
来源：http://chq.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://pon.ctjpmb.com

Java: resp.statusCode()
来源：http://dfb.hcnkem.com

Go:   resp.StatusCode
来源：http://qgs.svipenyu.cn

Ruby: resp.code.to_i
来源：http://dbx.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://qbb.nanxinkj.top

[L08] 并发请求多个地址
来源：http://dus.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mal.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://abr.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jrh.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwb.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pkg.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://quj.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kzg.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://peg.sysykeji.top

================================================================================
来源：http://jhb.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://rfw.dianchejie.cn

================================================================================
来源：http://zon.pycfn.com

[M01] 读取命令行参数
来源：http://scv.pycfn.com

Py:   sys.argv[1:]
来源：http://unv.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://qyt.birdmap.top

JS:   process.argv.slice(2)
来源：http://rqf.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://dkp.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://uyl.ydjk.org.cn

Go:   os.Args[1:]
来源：http://wul.daria6918.cn

Ruby: ARGV
来源：http://iod.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://tdk.jinqigfzy.top

[M02] 读取环境变量
来源：http://wxf.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://gni.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mir.yuxming.cn

JS:   process.env.HOME
来源：http://eiz.ivvv.top

TS:   process.env.HOME
来源：http://dfy.meibo888.top

Java: System.getenv("HOME")
来源：http://qwn.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ima.yj20258.top

Ruby: ENV["HOME"]
来源：http://oyi.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://enp.wangdashe.top

[M03] 执行外部命令
来源：http://hxr.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ddv.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cdw.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://izc.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ycr.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uwr.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://whv.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://sdx.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://hzl.guannengcc.top

[M04] 获取当前工作目录
来源：http://dgc.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://ang.vqdsnc.cn

PHP:  getcwd();
来源：http://hli.hcnkem.com

JS:   process.cwd()
来源：http://ovz.fanxiaobao.xyz

TS:   process.cwd()
来源：http://nrr.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://gev.pengpengdd.cyou

Go:   os.Getwd()
来源：http://rdj.xinyue.icu

Ruby: Dir.pwd
来源：http://eix.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rnp.dianchejie.cn

[M05] 设置退出码
来源：http://ltu.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://wce.shzxlz.cn

PHP:  exit(1);
来源：http://bxy.ppjwa.cn

JS:   process.exit(1)
来源：http://fjp.guowangkeji.top

TS:   process.exit(1)
来源：http://rkb.jinqigufen.top

Java: System.exit(1)
来源：http://ujo.uphjek.com

Go:   os.Exit(1)
来源：http://qpi.havefunace.top

Ruby: exit 1
来源：http://pyo.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvn.yj202588.top

[M06] 向标准错误输出
来源：http://vro.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://dhx.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qed.yfazqb.com

JS:   console.error("err")
来源：http://maa.c1oappe.top

TS:   console.error("err")
来源：http://pdy.hysaishi.cn

Java: System.err.println("err")
来源：http://lqn.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bes.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://tiw.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://hkl.cucudq.cn

[M07] 判断是否为主入口
来源：http://ccv.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://rvq.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rhl.gogol.net.cn

JS:   require.main === module
来源：http://ost.redwolf501.top

TS:   require.main === module
来源：http://wpx.yuxming.cn

Java: public static void main(String[] args)
来源：http://iqp.zhoulong.xyz

Go:   func main()
来源：http://vli.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bwn.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://rsw.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://spk.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://bsr.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://uzs.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://gqz.hywenlv.cn

TS:   process.platform;  process.version
来源：http://hey.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cad.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ycp.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ovq.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vxp.tian-w.cn

================================================================================
来源：http://nnl.wangdashe.top

N. 数据结构与算法
来源：http://vfq.jinqigfzy.top

================================================================================
来源：http://uof.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://nru.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://btn.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wjh.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wls.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xif.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://pon.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://osp.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cdq.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://epa.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://gys.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://nqm.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yyq.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ppd.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://nxk.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dox.hcnkem.com

Go:   slices.Sort(arr)
来源：http://ned.shzxlz.cn

Ruby: arr.sort
来源：http://gaz.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybm.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://sbc.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://orr.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://qdm.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsp.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kpt.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vkm.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lly.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qsj.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://crx.jianghu66.top

[N04] 斐波那契数列
来源：http://clo.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zpf.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zrs.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkk.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbq.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yma.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kum.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sme.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xqn.yueranfly.top

[N05] 最大公约数
来源：http://fdk.aizwys.cn

Py:   math.gcd(a, b)
来源：http://hyd.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wao.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zni.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://flv.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kuy.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sph.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://obq.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hyh.yuanzhike.top

[N06] 判断回文字符串
来源：http://oal.yj20258.top

Py:   s == s[::-1]
来源：http://wsc.sweek.top

PHP:  $s === strrev($s);
来源：http://ljk.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://jnl.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://nam.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lpm.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://sdm.daxiang520.top

Ruby: s == s.reverse
来源：http://jwr.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dxe.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://rqv.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ely.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zvr.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://twa.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://dpj.dashuyun.cn

Java: // 手写 HashMap
来源：http://vik.zycfv.cn

Go:   // 手写 map[int]int
来源：http://fre.cashguo.top

Ruby: // 手写 Hash
来源：http://nhj.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tsh.aizwys.cn

[N08] 生成全排列
来源：http://ezm.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://thu.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://fet.9152youxi.cn

JS:   // 手写回溯递归
来源：http://myz.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://gmq.cheryme.top

Java: // 手写回溯递归
来源：http://ldn.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://ymo.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://fls.xziqi.cn

C#:   // 手写回溯递归
来源：http://afv.zhixingplan.top

[N09] 栈与队列
来源：http://xvx.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gjj.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tqo.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lob.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mgf.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bkg.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://czk.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://arc.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://plo.hnxiangtu.top

[N10] 链表节点定义
来源：http://ndl.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xaa.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pif.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wuk.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lpi.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://yra.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aej.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yey.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ztq.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://cgq.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://txh.jqgfzy.top

PHP:  // 手写递归函数
来源：http://mcz.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://caq.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eaz.birdmap.top

Java: // 手写递归
来源：http://txq.dashuyun.cn

Go:   // 手写递归
来源：http://nox.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yjm.ctjpmb.com

C#:   // 手写递归
来源：http://rma.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mnp.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hop.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sah.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://een.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehx.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eaj.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dwq.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zrk.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xzc.ppjwa.cn

================================================================================
来源：http://ywr.xziqi.cn

O. 并发与异步
来源：http://ebe.fengsongda.top

================================================================================
来源：http://mdm.0kj1m.cn

[O01] 启动一个线程
来源：http://sya.gzhubu.top


<!-- 参考信息 -->