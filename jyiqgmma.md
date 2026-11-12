代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hgk.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xfc.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sma.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nfn.ybcxt.top

[K06] 解析 URL 查询串
来源：http://snm.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mhb.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://odv.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whv.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggy.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hub.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kmy.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ima.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ajs.cucudq.cn

[K07] 进制转换
来源：http://dov.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nth.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wfk.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bjq.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://egl.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xky.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xbu.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wbw.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mcx.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://xby.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://unx.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ryg.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://ldd.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://lpx.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fnu.hammf.cn

Go:   encoding/gob
来源：http://gud.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://wfs.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fdg.redwolf501.top

================================================================================
来源：http://vdb.0kj1m.cn

L. 网络请求
来源：http://afg.ydzc1.top

================================================================================
来源：http://pno.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://zab.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uxl.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hhi.birdmap.top

JS:   await fetch(url)
来源：http://fns.dashuyun.cn

TS:   await fetch(url)
来源：http://aqv.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bia.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://rmc.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://kfa.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jdh.zhengqikj.top

[L02] 发送 POST JSON
来源：http://hcj.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://isq.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tvo.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eth.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjv.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jyc.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yng.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xpy.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pfh.zhengqikj.top

[L03] 设置自定义请求头
来源：http://vso.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pks.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oou.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qzs.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ouk.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://umg.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vlc.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zod.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dml.daria6918.cn

[L04] 设置超时
来源：http://kre.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://ktp.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgt.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvn.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyo.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vzj.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fhx.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rvz.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kyv.tian-w.cn

[L05] 上传文件（multipart）
来源：http://afs.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qub.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wyl.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://maq.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xww.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uxu.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vfb.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cys.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://snl.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://ocm.hongshengwenyu.top

Py:   resp.json()
来源：http://dsk.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://suu.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://kme.epnwcf.com

TS:   await resp.json()
来源：http://ybh.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fef.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cdf.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://vxh.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://odt.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://whb.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tnc.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://apj.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://ivd.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://bup.yj202588.top

Java: resp.statusCode()
来源：http://evh.gzhubu.top

Go:   resp.StatusCode
来源：http://veu.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://xzj.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://iln.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://wiu.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kcn.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://pmd.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rir.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gus.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dws.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://okg.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qgl.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lwd.birdmap.top

================================================================================
来源：http://lex.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://drc.52xcode.cn

================================================================================
来源：http://evi.kuanghao11.cn

[M01] 读取命令行参数
来源：http://dzr.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://byr.shuidangran.top

PHP:  $argv;  $argc;
来源：http://xmz.havefunace.top

JS:   process.argv.slice(2)
来源：http://cmt.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://jnm.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://sss.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://bpz.ydzc1.top

Ruby: ARGV
来源：http://bif.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://gle.yj20258888.top

[M02] 读取环境变量
来源：http://wqr.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://xgp.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://brn.gaohongyu789.top

JS:   process.env.HOME
来源：http://ylw.gotoacloud.top

TS:   process.env.HOME
来源：http://irm.yfazqb.com

Java: System.getenv("HOME")
来源：http://coq.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ehn.hcnkem.com

Ruby: ENV["HOME"]
来源：http://zav.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yao.guannengcc.top

[M03] 执行外部命令
来源：http://lww.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qqc.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uxm.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hqb.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yug.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wco.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://imr.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://duh.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://gvp.tarul.cn

[M04] 获取当前工作目录
来源：http://dny.chenlongwang.top

Py:   os.getcwd()
来源：http://ssa.feifeiyinyue.top

PHP:  getcwd();
来源：http://rwa.cucudq.cn

JS:   process.cwd()
来源：http://drf.epnwcf.com

TS:   process.cwd()
来源：http://hrf.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://icg.svipenyu.cn

Go:   os.Getwd()
来源：http://oon.zhoulong.xyz

Ruby: Dir.pwd
来源：http://cvm.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://yip.jiagoushi.top

[M05] 设置退出码
来源：http://ydv.fktsv.cn

Py:   sys.exit(1)
来源：http://tvx.fktsv.cn

PHP:  exit(1);
来源：http://ebv.tanke756.top

JS:   process.exit(1)
来源：http://prg.hammf.cn

TS:   process.exit(1)
来源：http://amn.sysykeji.top

Java: System.exit(1)
来源：http://ntd.sysykeji.top

Go:   os.Exit(1)
来源：http://vpq.daxiang520.top

Ruby: exit 1
来源：http://wrk.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dix.dianchejie.cn

[M06] 向标准错误输出
来源：http://meb.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://knn.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fjm.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://jnw.jqgufenzy.top

TS:   console.error("err")
来源：http://yqb.gzhubu.top

Java: System.err.println("err")
来源：http://zvm.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fpb.havefunace.top

Ruby: warn "err"
来源：http://jse.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://khf.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://cjy.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://ume.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bmf.shuidangran.top

JS:   require.main === module
来源：http://tfo.gotoacloud.top

TS:   require.main === module
来源：http://pxi.yj20258.top

Java: public static void main(String[] args)
来源：http://tdm.xinyue.icu

Go:   func main()
来源：http://yxw.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zww.fehbvm.com

C#:   static void Main(string[] args)
来源：http://qdc.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://lht.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://ekv.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://zuh.mhx1999.top

JS:   process.platform;  process.version
来源：http://rhb.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://yiy.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ydi.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wsk.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://djv.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ooi.redwolf501.top

================================================================================
来源：http://owe.yj202588.top

N. 数据结构与算法
来源：http://drx.tarul.cn

================================================================================
来源：http://rop.tarul.cn

[N01] 二分查找（有序数组）
来源：http://tsm.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://biv.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rru.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msv.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwt.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://wjx.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://yiz.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijp.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bgx.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://fvs.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://llc.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sdj.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vtt.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wqv.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eda.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://kir.jiagoushi.top

Ruby: arr.sort
来源：http://vtn.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxd.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://qrk.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nuy.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://smx.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ctp.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kau.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ynf.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bxa.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://njm.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://tuh.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://hxc.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zzb.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ccm.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vod.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://clh.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nyr.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hcg.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dle.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vug.redwolf501.top

[N05] 最大公约数
来源：http://fdm.mhx1999.top

Py:   math.gcd(a, b)
来源：http://frr.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dqm.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqa.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kki.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ozr.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fbm.yonumen.top

Ruby: a.gcd(b)
来源：http://yea.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kok.xylfe.cn

[N06] 判断回文字符串
来源：http://lyr.meibo888.top

Py:   s == s[::-1]
来源：http://qar.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://urb.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://rnh.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://zma.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ryc.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://vnz.fzhhl.top

Ruby: s == s.reverse
来源：http://nuc.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eit.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://joo.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vme.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nme.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qbo.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://lxt.ppjwa.cn

Java: // 手写 HashMap
来源：http://zzn.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://ttg.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://nlm.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ifk.yueranfly.top

[N08] 生成全排列
来源：http://tjr.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://atc.ehwqpu.com

PHP:  // 手写递归交换
来源：http://lvs.cheryme.top

JS:   // 手写回溯递归
来源：http://cfg.xinyue.icu

TS:   // 手写回溯递归
来源：http://xat.quarkkingdee.top

Java: // 手写回溯递归
来源：http://zym.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://vxa.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://buo.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://gpb.yuanzhike.top

[N09] 栈与队列
来源：http://xep.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pwk.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pyb.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qar.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghw.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pvt.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://che.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zno.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mim.hcnkem.com

[N10] 链表节点定义
来源：http://nfg.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xiv.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://znq.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jko.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gbl.cheryme.top

Java: class Node { int v; Node next; }
来源：http://qsf.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://spk.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vjg.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vyc.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://ldj.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hqo.andypj.xyz

PHP:  // 手写递归函数
来源：http://kvd.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlr.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nod.gzhubu.top

Java: // 手写递归
来源：http://ewf.svipenyu.cn

Go:   // 手写递归
来源：http://iaa.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kfs.tarul.cn

C#:   // 手写递归
来源：http://fdy.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sws.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kqn.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tyk.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbg.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ywt.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oza.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pne.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fxw.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dol.haohaochexian.top

================================================================================
来源：http://dnp.gzhubu.top

O. 并发与异步
来源：http://xiu.birdmap.top

================================================================================
来源：http://ztr.redwolf501.top

[O01] 启动一个线程
来源：http://gbg.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lpv.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://akx.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://orx.meibo888.top

TS:   // 同 JS
来源：http://izb.nwbrower.top


<!-- 参考信息 -->