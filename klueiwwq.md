代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fpm.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vfa.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fdv.yanxiufei.cn

[K05] 深拷贝对象
来源：http://xzh.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://qmy.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://pwo.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://djg.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://pbl.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zvd.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://owk.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ejd.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hpj.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://bas.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ljg.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zse.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dja.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plu.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rmj.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oyh.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bni.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yfl.ydzc1.top

[K07] 进制转换
来源：http://hfh.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vub.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aus.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qhp.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mvf.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tiz.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jnb.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uvs.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://woo.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://pht.pycfn.com

Py:   pickle.dumps(obj)
来源：http://gbf.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uks.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://ksf.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://ian.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://syh.hnqzz.top

Go:   encoding/gob
来源：http://zli.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://juv.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hjv.dianchejie.cn

================================================================================
来源：http://bcq.ivvv.top

L. 网络请求
来源：http://dla.daria6918.cn

================================================================================
来源：http://wue.sysykeji.top

[L01] 发送 GET 请求
来源：http://xyf.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sih.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dwu.nwbrower.top

JS:   await fetch(url)
来源：http://gmr.yj20258.top

TS:   await fetch(url)
来源：http://kwl.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wnd.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://brv.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://huy.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pqu.yonumen.top

[L02] 发送 POST JSON
来源：http://urk.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://mkt.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://luk.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppy.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhw.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrn.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gxa.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://giv.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yur.yj20258.top

[L03] 设置自定义请求头
来源：http://sbw.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eoi.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zlc.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijl.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ler.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zxd.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zpi.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nlq.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vwd.chenzaomai.com

[L04] 设置超时
来源：http://wmq.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://jdp.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ree.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kze.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpx.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vyy.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czu.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vmz.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxd.guannengcc.top

[L05] 上传文件（multipart）
来源：http://bio.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hsb.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://prg.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mlq.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fhe.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cpg.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ium.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bei.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eld.ybcxt.top

[L06] 解析响应为 JSON
来源：http://dge.havefunace.top

Py:   resp.json()
来源：http://qtj.shuidangran.top

PHP:  json_decode($body, true);
来源：http://aot.ybcxt.top

JS:   await resp.json()
来源：http://fhv.chenzaomai.com

TS:   await resp.json()
来源：http://hmu.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hcq.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tyx.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://bqn.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://luo.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://xbj.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wze.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mrt.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://knf.tanke756.top

TS:   resp.ok;  resp.status
来源：http://cbi.zhoulong.xyz

Java: resp.statusCode()
来源：http://zga.jinqigfzy.top

Go:   resp.StatusCode
来源：http://naj.gzhubu.top

Ruby: resp.code.to_i
来源：http://lfn.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://ptr.ybcxt.top

[L08] 并发请求多个地址
来源：http://jdo.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://adj.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://hrx.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jlt.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzn.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wda.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bih.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nzr.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pav.yfazqb.com

================================================================================
来源：http://kkj.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://ixl.yj20258.top

================================================================================
来源：http://ngk.birdmap.top

[M01] 读取命令行参数
来源：http://vdp.wangdashe.top

Py:   sys.argv[1:]
来源：http://kaj.daria6918.cn

PHP:  $argv;  $argc;
来源：http://efq.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://uvg.fehbvm.com

TS:   process.argv.slice(2)
来源：http://ezx.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://oir.xuanzx.com

Go:   os.Args[1:]
来源：http://cim.fktsv.cn

Ruby: ARGV
来源：http://loy.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://ovb.ehwqpu.com

[M02] 读取环境变量
来源：http://ilp.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://wvb.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xyp.hysaishi.cn

JS:   process.env.HOME
来源：http://khm.yfazqb.com

TS:   process.env.HOME
来源：http://yls.cheryme.top

Java: System.getenv("HOME")
来源：http://tyk.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jur.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://efl.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vhl.fehbvm.com

[M03] 执行外部命令
来源：http://eaq.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://olp.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czt.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mwi.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bcr.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aim.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://zcc.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gid.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://qul.cheryme.top

[M04] 获取当前工作目录
来源：http://lqs.9152youxi.cn

Py:   os.getcwd()
来源：http://agg.hfpthk.cn

PHP:  getcwd();
来源：http://izv.tanke756.top

JS:   process.cwd()
来源：http://egh.sjlbkw.cn

TS:   process.cwd()
来源：http://tot.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://duz.wangshuangyany.cn

Go:   os.Getwd()
来源：http://ivx.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://umq.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://nsg.chenzaomai.com

[M05] 设置退出码
来源：http://mhw.dianchejie.cn

Py:   sys.exit(1)
来源：http://voo.feifeiyinyue.top

PHP:  exit(1);
来源：http://syf.xylfe.cn

JS:   process.exit(1)
来源：http://dip.9152youxi.cn

TS:   process.exit(1)
来源：http://eed.c1oappe.top

Java: System.exit(1)
来源：http://mbb.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://qox.redwolf501.top

Ruby: exit 1
来源：http://xzr.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oli.316326.xyz

[M06] 向标准错误输出
来源：http://szj.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://iwa.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gkg.nwbrower.top

JS:   console.error("err")
来源：http://lct.daxiang520.top

TS:   console.error("err")
来源：http://byg.0kj1m.cn

Java: System.err.println("err")
来源：http://oup.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://umg.vqdsnc.cn

Ruby: warn "err"
来源：http://fzq.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://wpe.yongpay.top

[M07] 判断是否为主入口
来源：http://zkk.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://oyt.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xpz.redwolf501.top

JS:   require.main === module
来源：http://geh.gotoacloud.top

TS:   require.main === module
来源：http://sie.yfazqb.com

Java: public static void main(String[] args)
来源：http://iqk.ctjpmb.com

Go:   func main()
来源：http://hhr.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mvi.fzhhl.top

C#:   static void Main(string[] args)
来源：http://eyp.sweek.top

[M08] 获取系统与运行时信息
来源：http://nvp.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://ala.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://nrq.yueranfly.top

JS:   process.platform;  process.version
来源：http://edr.aibaodan.cn

TS:   process.platform;  process.version
来源：http://yaj.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fmx.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://obo.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hxg.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xbd.yanxiufei.cn

================================================================================
来源：http://vim.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://zmb.dashuyun.cn

================================================================================
来源：http://bwb.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://ktz.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qsp.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pcd.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vij.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wjf.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://lhe.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://gie.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rct.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://yas.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cet.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://wva.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gcw.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://umv.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fcx.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eyq.xuanzx.com

Go:   slices.Sort(arr)
来源：http://xsp.birdmap.top

Ruby: arr.sort
来源：http://odc.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xvh.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://jok.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://emf.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://obm.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oog.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://akj.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gep.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhh.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://osl.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://drt.cheryme.top

[N04] 斐波那契数列
来源：http://qyr.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dzb.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pss.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://avf.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivj.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trq.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xgw.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ihc.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vub.yuanzhike.top

[N05] 最大公约数
来源：http://foc.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://aav.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gdy.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzt.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffm.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbk.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cby.aibaodan.cn

Ruby: a.gcd(b)
来源：http://yuc.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zfi.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://yoy.tanke756.top

Py:   s == s[::-1]
来源：http://btu.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://nbq.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://dlr.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://sbc.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fkk.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://iio.svipenyu.cn

Ruby: s == s.reverse
来源：http://ojd.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpi.sweek.top

[N07] 两数之和（返回下标）
来源：http://anf.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://alp.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://udk.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://myp.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://vie.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://pua.epnwcf.com

Go:   // 手写 map[int]int
来源：http://lyy.smart0.xyz

Ruby: // 手写 Hash
来源：http://fiv.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ncx.jqgfzy.top

[N08] 生成全排列
来源：http://kvv.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://stp.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://psy.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://zcw.birdmap.top

TS:   // 手写回溯递归
来源：http://ake.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://rmm.sysykeji.top

Go:   // 手写回溯递归
来源：http://ouz.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://bsc.shzxlz.cn

C#:   // 手写回溯递归
来源：http://xxf.nanxinkj.top

[N09] 栈与队列
来源：http://fwl.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oic.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gua.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dmn.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aom.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sav.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rrg.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jbc.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jsp.gzhubu.top

[N10] 链表节点定义
来源：http://rrc.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gik.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pgw.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mtc.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qkq.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://vmz.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ijc.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qvo.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pwd.hesvh.cn

[N11] 二叉树中序遍历
来源：http://cvq.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://obp.chenlongwang.top

PHP:  // 手写递归函数
来源：http://yxk.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnh.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kee.hnqzz.top

Java: // 手写递归
来源：http://vay.hnxiangtu.top

Go:   // 手写递归
来源：http://qvg.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uxx.shzxlz.cn

C#:   // 手写递归
来源：http://rnl.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://khw.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thu.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zqu.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uea.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fuf.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ovc.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tqa.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hvh.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sso.jqgfzy.top


<!-- 参考信息 -->