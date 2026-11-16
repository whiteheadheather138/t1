代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://qvc.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jod.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zbw.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ohm.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://kgl.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://prl.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wza.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkk.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvn.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ngx.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jyt.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://doe.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ngc.feifeiyinyue.top

[K07] 进制转换
来源：http://har.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lss.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jem.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vem.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ann.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wzp.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rit.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ayv.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wtv.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://utf.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://hpc.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cjz.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://hty.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://qbo.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://epl.jqgufenzy.top

Go:   encoding/gob
来源：http://ozj.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://jqh.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ibz.cashguo.top

================================================================================
来源：http://vnn.gogol.net.cn

L. 网络请求
来源：http://eme.shanyushiyangkeji.top

================================================================================
来源：http://jat.zycfv.cn

[L01] 发送 GET 请求
来源：http://jsa.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lgd.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hbs.tian-w.cn

JS:   await fetch(url)
来源：http://kad.guowangkeji.top

TS:   await fetch(url)
来源：http://nfk.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ldm.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://vhw.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fsp.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fwc.bjfxy.top

[L02] 发送 POST JSON
来源：http://ela.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://owc.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qza.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbv.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://arj.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fou.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ncu.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mpg.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lbo.yonumen.top

[L03] 设置自定义请求头
来源：http://woq.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ava.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tgg.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vba.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fss.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bjp.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xvk.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cjp.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uos.nanxinkj.top

[L04] 设置超时
来源：http://vrp.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://diu.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzi.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltg.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rid.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rdc.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ist.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sjf.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://brm.ivvv.top

[L05] 上传文件（multipart）
来源：http://wsa.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ndh.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nlf.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tim.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kjn.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayy.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cjo.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gyg.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wpp.hammf.cn

[L06] 解析响应为 JSON
来源：http://raf.cdnleiting.top

Py:   resp.json()
来源：http://qaa.fehbvm.com

PHP:  json_decode($body, true);
来源：http://sil.redwolf501.top

JS:   await resp.json()
来源：http://jkr.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://rqy.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tfm.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xvo.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://xpc.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vgu.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://cjy.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://olk.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyv.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://ycv.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://jij.sysykeji.top

Java: resp.statusCode()
来源：http://pwj.yfazqb.com

Go:   resp.StatusCode
来源：http://qsv.vehdjk.com

Ruby: resp.code.to_i
来源：http://fue.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://tcm.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://yvg.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lbf.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://afx.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ora.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wca.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ocv.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xcl.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ekm.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kys.zhaomingkeji.xyz

================================================================================
来源：http://jfb.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://elh.zhaomingkeji.xyz

================================================================================
来源：http://ube.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://sik.daria6918.cn

Py:   sys.argv[1:]
来源：http://hgy.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://zmz.jianghu66.top

JS:   process.argv.slice(2)
来源：http://rkb.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://jur.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://rdr.vehdjk.com

Go:   os.Args[1:]
来源：http://xjw.sufxvd.cn

Ruby: ARGV
来源：http://wkh.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://ior.yj20258.top

[M02] 读取环境变量
来源：http://wuo.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://xin.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pdy.hnxiangtu.top

JS:   process.env.HOME
来源：http://ude.zhiwuduotai.top

TS:   process.env.HOME
来源：http://msz.wangdashe.top

Java: System.getenv("HOME")
来源：http://yjp.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hft.meibo888.top

Ruby: ENV["HOME"]
来源：http://txh.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zhg.yuanzhike.top

[M03] 执行外部命令
来源：http://hyg.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mrn.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ebm.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://rjk.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hbg.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://scc.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uet.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rxi.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://iob.ybcxt.top

[M04] 获取当前工作目录
来源：http://kvo.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://qdp.jinqigufen.top

PHP:  getcwd();
来源：http://mlu.zhongyouzk.top

JS:   process.cwd()
来源：http://vnj.xylfe.cn

TS:   process.cwd()
来源：http://bai.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://vut.nanxinkj.top

Go:   os.Getwd()
来源：http://ucv.smart0.xyz

Ruby: Dir.pwd
来源：http://igb.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pyf.sysykeji.top

[M05] 设置退出码
来源：http://hzo.redwolf501.top

Py:   sys.exit(1)
来源：http://fgx.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://stv.nanxinkj.top

JS:   process.exit(1)
来源：http://zdt.hongshengwenyu.top

TS:   process.exit(1)
来源：http://smn.jinqigfzy.top

Java: System.exit(1)
来源：http://ehs.sxryk.cn

Go:   os.Exit(1)
来源：http://wvd.cdnleiting.top

Ruby: exit 1
来源：http://pyz.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kxl.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://qxh.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://jxb.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iyk.cqqwz.cn

JS:   console.error("err")
来源：http://kav.fehbvm.com

TS:   console.error("err")
来源：http://pze.gaohongyu789.top

Java: System.err.println("err")
来源：http://ath.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ovf.meibo888.top

Ruby: warn "err"
来源：http://vvi.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://oga.tian-w.cn

[M07] 判断是否为主入口
来源：http://dnp.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://dxz.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqa.dianchejie.cn

JS:   require.main === module
来源：http://qyy.c1oappe.top

TS:   require.main === module
来源：http://tdt.aibaodan.cn

Java: public static void main(String[] args)
来源：http://isp.xingfuxueyuan.xyz

Go:   func main()
来源：http://mim.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uac.yj20258.top

C#:   static void Main(string[] args)
来源：http://usu.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://fju.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://mmz.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://gra.dianchejie.cn

JS:   process.platform;  process.version
来源：http://ajg.sufxvd.cn

TS:   process.platform;  process.version
来源：http://luh.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rve.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://irr.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pfb.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lif.guowangkeji.top

================================================================================
来源：http://sgl.havefunace.top

N. 数据结构与算法
来源：http://ggl.yvedp.cn

================================================================================
来源：http://lgq.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://fyl.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cgi.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ubb.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gbx.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwu.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://hrj.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://shn.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lmf.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://unk.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://izd.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://czz.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cqn.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tvb.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://rwo.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uqg.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://wdc.shangyingyoupin.top

Ruby: arr.sort
来源：http://vvv.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ahv.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://jpy.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dgl.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://fvx.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tlh.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ydq.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lne.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ogq.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nhl.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://jwh.aizwys.cn

[N04] 斐波那契数列
来源：http://zmv.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gqg.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iob.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tat.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cwq.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cpn.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rhw.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oet.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tae.hfpthk.cn

[N05] 最大公约数
来源：http://iyo.fengsongda.top

Py:   math.gcd(a, b)
来源：http://wdi.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mkb.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://llz.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfm.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ogm.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dvb.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://zmz.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvr.ctjpmb.com

[N06] 判断回文字符串
来源：http://hpk.gotoacloud.top

Py:   s == s[::-1]
来源：http://fth.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://sap.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://bfr.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://xuh.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://scp.guannengcc.top

Go:   // 双指针从两端比较
来源：http://okx.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://map.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oco.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://eru.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tiu.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fir.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xrv.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://trf.hywenlv.cn

Java: // 手写 HashMap
来源：http://szq.mhx1999.top

Go:   // 手写 map[int]int
来源：http://gfd.sufxvd.cn

Ruby: // 手写 Hash
来源：http://erk.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://igl.shzxlz.cn

[N08] 生成全排列
来源：http://tsl.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://mew.ctjpmb.com

PHP:  // 手写递归交换
来源：http://kkg.gogol.net.cn

JS:   // 手写回溯递归
来源：http://rjo.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://ywi.yfazqb.com

Java: // 手写回溯递归
来源：http://fnb.jyoumei.cn

Go:   // 手写回溯递归
来源：http://lkm.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://qni.ppjwa.cn

C#:   // 手写回溯递归
来源：http://pox.guannengcc.top

[N09] 栈与队列
来源：http://kls.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nau.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cby.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rey.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvv.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yxk.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pmo.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkn.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://enx.bbcook.cn

[N10] 链表节点定义
来源：http://kpk.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ldx.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hyz.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mhv.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rhx.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://itc.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://avq.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xbs.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qqw.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://vrm.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tbs.zdqjudy.top

PHP:  // 手写递归函数
来源：http://kef.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hye.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ynr.dianchejie.cn

Java: // 手写递归
来源：http://uor.vehdjk.com

Go:   // 手写递归
来源：http://wze.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kcm.shanyushiyangtech.top

C#:   // 手写递归
来源：http://oeb.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://czm.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rqf.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvn.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvm.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kwm.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uim.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bgx.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vzx.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kpj.gotoacloud.top

================================================================================
来源：http://xtq.cucudq.cn

O. 并发与异步
来源：http://igh.jyoumei.cn

================================================================================
来源：http://tpe.guowangkeji.top

[O01] 启动一个线程
来源：http://ybs.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ctk.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zjz.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bla.jinqigufen.top

TS:   // 同 JS
来源：http://pcc.jinyuanbaomall.cn


<!-- 参考信息 -->