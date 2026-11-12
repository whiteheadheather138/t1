代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://fcc.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://fvs.iojbl.cn

JS:   structuredClone(obj)
来源：http://qoy.xuetiantiany.cn

TS:   structuredClone(obj)
来源：http://tjj.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ovm.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogt.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qki.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aoy.yongpay.top

[K06] 解析 URL 查询串
来源：http://tuc.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yqx.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://enn.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kzr.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpo.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygj.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gcu.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lyc.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://poi.gzhubu.top

[K07] 进制转换
来源：http://faz.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kuf.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xqx.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dig.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://grm.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ytv.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dxt.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eqv.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ens.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://oln.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://dta.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cvz.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://cpi.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://ird.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://utj.hywenlv.cn

Go:   encoding/gob
来源：http://dzb.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://avb.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjq.cucudq.cn

================================================================================
来源：http://agf.hfpthk.cn

L. 网络请求
来源：http://lhz.birdmap.top

================================================================================
来源：http://mqo.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://owi.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mxe.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ffy.daxiang520.top

JS:   await fetch(url)
来源：http://umt.nwbrower.top

TS:   await fetch(url)
来源：http://hbz.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lal.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://yxk.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kuc.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qai.52xcode.cn

[L02] 发送 POST JSON
来源：http://nvw.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yrt.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hsq.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jzl.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bfv.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vzn.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wsv.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vfp.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kux.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://olr.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xja.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wzp.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yxp.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qvw.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://icq.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dfp.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbs.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nhv.jinqigufen.top

[L04] 设置超时
来源：http://lfo.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://bjl.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mzz.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xpm.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxj.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odc.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ams.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jju.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cyc.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://thh.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://frz.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dlr.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jas.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qej.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cpp.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dyi.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngx.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uah.sysykeji.top

[L06] 解析响应为 JSON
来源：http://das.ehwqpu.com

Py:   resp.json()
来源：http://irn.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://yqy.vqdsnc.cn

JS:   await resp.json()
来源：http://qbi.yuxming.cn

TS:   await resp.json()
来源：http://wig.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lqe.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lgz.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://usg.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gvj.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://cbo.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kjl.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rab.316326.xyz

JS:   resp.ok;  resp.status
来源：http://lor.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://yqy.wangdashe.top

Java: resp.statusCode()
来源：http://pqs.cashguo.top

Go:   resp.StatusCode
来源：http://txb.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://jlr.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://iqf.hnqzz.top

[L08] 并发请求多个地址
来源：http://omq.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ves.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://btv.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqk.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://onj.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kdp.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mno.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xmv.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nfh.yangfankeji.com

================================================================================
来源：http://dse.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://yvy.xylfe.cn

================================================================================
来源：http://jqi.wangdashe.top

[M01] 读取命令行参数
来源：http://taw.ybcxt.top

Py:   sys.argv[1:]
来源：http://lll.fzhhl.top

PHP:  $argv;  $argc;
来源：http://ahl.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://zip.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://nkj.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://aoi.meibo888.top

Go:   os.Args[1:]
来源：http://ixq.jiagoushi.top

Ruby: ARGV
来源：http://qyu.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://oha.xylfe.cn

[M02] 读取环境变量
来源：http://sia.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://cin.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://egy.nanxinkj.top

JS:   process.env.HOME
来源：http://kds.ydjk.org.cn

TS:   process.env.HOME
来源：http://ogt.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://vxy.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://usn.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://xvv.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://azd.52xcode.cn

[M03] 执行外部命令
来源：http://hyc.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dso.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vod.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://wrc.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xlb.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tfq.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://imt.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://zho.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://izb.havefunace.top

[M04] 获取当前工作目录
来源：http://wrj.jianghu66.top

Py:   os.getcwd()
来源：http://xvt.52xcode.cn

PHP:  getcwd();
来源：http://sas.zycfv.cn

JS:   process.cwd()
来源：http://hmo.shzxlz.cn

TS:   process.cwd()
来源：http://tlp.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://wds.bbcook.cn

Go:   os.Getwd()
来源：http://jrb.hcnkem.com

Ruby: Dir.pwd
来源：http://ddv.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dvl.zdqjudy.top

[M05] 设置退出码
来源：http://zoq.zhengqikj.top

Py:   sys.exit(1)
来源：http://arq.yvedp.cn

PHP:  exit(1);
来源：http://mvz.xuanzx.com

JS:   process.exit(1)
来源：http://idn.tanke756.top

TS:   process.exit(1)
来源：http://cfe.hongshengwenyu.top

Java: System.exit(1)
来源：http://nkr.zhoulong.xyz

Go:   os.Exit(1)
来源：http://kcx.zhaomingkeji.xyz

Ruby: exit 1
来源：http://tux.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kkd.haohaochexian.top

[M06] 向标准错误输出
来源：http://tcd.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://vvz.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xnm.aibaodan.cn

JS:   console.error("err")
来源：http://row.yj202588.top

TS:   console.error("err")
来源：http://wol.xuetiantiany.cn

Java: System.err.println("err")
来源：http://shi.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kfe.jyoumei.cn

Ruby: warn "err"
来源：http://kdh.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://okf.shzxlz.cn

[M07] 判断是否为主入口
来源：http://gig.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://yga.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gbw.smart0.xyz

JS:   require.main === module
来源：http://tvc.zhongyouzk.top

TS:   require.main === module
来源：http://imm.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://icq.fktsv.cn

Go:   func main()
来源：http://sxt.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oty.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://cqa.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://wad.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://xet.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://kmv.tanke756.top

JS:   process.platform;  process.version
来源：http://wsk.52xcode.cn

TS:   process.platform;  process.version
来源：http://vfu.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhw.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dac.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://acu.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://arc.wangshuangyany.cn

================================================================================
来源：http://xji.xuanzx.com

N. 数据结构与算法
来源：http://rgs.gogol.net.cn

================================================================================
来源：http://iaf.havefunace.top

[N01] 二分查找（有序数组）
来源：http://jsq.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://dnw.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rct.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggv.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rdx.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://tvg.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://csu.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://whn.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://vek.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://tqe.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://wwh.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rcg.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://utd.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tzd.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tnq.tarul.cn

Go:   slices.Sort(arr)
来源：http://oyt.0kj1m.cn

Ruby: arr.sort
来源：http://tnp.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qnw.pycfn.com

[N03] 快速排序（分治示例）
来源：http://hlh.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ypl.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://fpl.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://auo.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqx.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msd.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eum.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://avh.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://lej.hfpthk.cn

[N04] 斐波那契数列
来源：http://xdz.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://anh.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yhb.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://icj.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bhy.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wfd.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aab.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vys.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znf.hnqzz.top

[N05] 最大公约数
来源：http://syt.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://zlv.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nqo.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvx.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nca.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ram.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vtz.meibo888.top

Ruby: a.gcd(b)
来源：http://glp.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wir.gotoacloud.top

[N06] 判断回文字符串
来源：http://fqs.shuidangran.top

Py:   s == s[::-1]
来源：http://obh.smart0.xyz

PHP:  $s === strrev($s);
来源：http://oqw.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://vmd.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://ejs.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kda.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://dni.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://wop.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://aee.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://umx.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gzj.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cte.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://fhq.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://xtm.jqgufenzy.top

Java: // 手写 HashMap
来源：http://cis.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://oqg.cdnleiting.top

Ruby: // 手写 Hash
来源：http://znv.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://rui.jinqigufen.top

[N08] 生成全排列
来源：http://uqm.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://zil.yuanzhike.top

PHP:  // 手写递归交换
来源：http://yil.jqgfzy.top

JS:   // 手写回溯递归
来源：http://guh.gotoacloud.top

TS:   // 手写回溯递归
来源：http://cus.zdbjq.cn

Java: // 手写回溯递归
来源：http://chk.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://ukw.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://mhh.jqgfzy.top

C#:   // 手写回溯递归
来源：http://nbt.dianchejie.cn

[N09] 栈与队列
来源：http://zdp.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vds.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pls.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jtt.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zbh.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwb.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fqu.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qlj.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wix.cucudq.cn

[N10] 链表节点定义
来源：http://gfq.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rvl.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tie.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jgv.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://erp.ivvv.top

Java: class Node { int v; Node next; }
来源：http://pmp.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://nmk.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cwb.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bzy.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://tim.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tnl.sysykeji.top

PHP:  // 手写递归函数
来源：http://onh.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ezd.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://npn.svipenyu.cn

Java: // 手写递归
来源：http://kmi.yueranfly.top

Go:   // 手写递归
来源：http://jpn.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kzx.yj20258888.top

C#:   // 手写递归
来源：http://tfq.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kow.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pbh.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zjr.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wek.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dyx.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dks.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://snk.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aks.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygd.meibo888.top

================================================================================
来源：http://lgs.dianchejie.cn

O. 并发与异步
来源：http://geb.zdqjudy.top

================================================================================
来源：http://zol.chenjidiqi.icu

[O01] 启动一个线程
来源：http://one.jlsjyb.cn


<!-- 参考信息 -->