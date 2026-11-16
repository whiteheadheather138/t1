代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ekt.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://ymk.xinyue.icu

JS:   structuredClone(obj)
来源：http://kjv.redwolf501.top

TS:   structuredClone(obj)
来源：http://wbu.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://uws.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zgd.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uoq.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qfh.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://dxz.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pvr.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ilj.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://flg.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgf.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wyv.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uyh.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nuk.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jdf.yuanzhike.top

[K07] 进制转换
来源：http://qnt.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ckk.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vmc.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kzh.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ixm.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rbr.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nrl.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rkz.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lqi.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://zsv.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://xfp.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://sqj.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://dky.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://yoq.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://shg.ydjk.org.cn

Go:   encoding/gob
来源：http://frf.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://spk.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://opr.gaohongyu789.top

================================================================================
来源：http://hcb.jinyuanbaomall.cn

L. 网络请求
来源：http://syj.iojbl.cn

================================================================================
来源：http://oxw.nanxinkj.top

[L01] 发送 GET 请求
来源：http://uvj.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vmt.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eow.zhongyouzk.top

JS:   await fetch(url)
来源：http://emn.ctjpmb.com

TS:   await fetch(url)
来源：http://auu.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eth.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://ygw.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ete.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://srm.cheryme.top

[L02] 发送 POST JSON
来源：http://tbl.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iud.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ndh.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkt.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dlf.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dhj.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qdt.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uzv.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tcq.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://pei.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://szv.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hqp.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nmj.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xft.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqn.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cvs.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nxz.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bul.shangyingyoupin.top

[L04] 设置超时
来源：http://quq.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://dtz.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lpy.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://agx.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ncx.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pnb.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fgi.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kzz.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://grm.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://bfx.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://phc.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lhf.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zrs.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kiw.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wxm.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://btk.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qhc.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lsr.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://svp.zhoulong.xyz

Py:   resp.json()
来源：http://uyv.hnqzz.top

PHP:  json_decode($body, true);
来源：http://ibu.epnwcf.com

JS:   await resp.json()
来源：http://ivd.meibo888.top

TS:   await resp.json()
来源：http://dtn.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wua.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bwm.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://bzh.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jac.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://qgc.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pvf.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ivw.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://fbv.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://nbb.yuxming.cn

Java: resp.statusCode()
来源：http://ikh.ydzc1.top

Go:   resp.StatusCode
来源：http://ejy.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://dtz.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://bzq.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://emo.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://heo.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://ppr.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fsn.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://muj.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mvy.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmf.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wjk.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rzt.ctjpmb.com

================================================================================
来源：http://pcj.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://dui.xuetiantiany.cn

================================================================================
来源：http://rvn.yangfankeji.com

[M01] 读取命令行参数
来源：http://ipy.meibo888.top

Py:   sys.argv[1:]
来源：http://ckh.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://jcz.fehbvm.com

JS:   process.argv.slice(2)
来源：http://hzd.tarul.cn

TS:   process.argv.slice(2)
来源：http://hrv.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://iii.9152youxi.cn

Go:   os.Args[1:]
来源：http://sgv.sysykeji.top

Ruby: ARGV
来源：http://yrt.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://yyo.ctjpmb.com

[M02] 读取环境变量
来源：http://oev.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://adq.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xng.havefunace.top

JS:   process.env.HOME
来源：http://glv.yuanzhike.top

TS:   process.env.HOME
来源：http://vum.sysykeji.top

Java: System.getenv("HOME")
来源：http://zzh.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bqe.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://nad.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kvq.zdbjq.cn

[M03] 执行外部命令
来源：http://thp.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sje.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vfs.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nja.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vxg.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wmo.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://oxm.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cqc.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://mvh.yj20258.top

[M04] 获取当前工作目录
来源：http://pqs.chenzaomai.com

Py:   os.getcwd()
来源：http://szr.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://fkb.sysykeji.top

JS:   process.cwd()
来源：http://qkj.zhengqikj.top

TS:   process.cwd()
来源：http://byn.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://wug.9152youxi.cn

Go:   os.Getwd()
来源：http://lqk.nwbrower.top

Ruby: Dir.pwd
来源：http://wif.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://vzb.jinghuilouyu.cn

[M05] 设置退出码
来源：http://ebx.jinqigfzy.top

Py:   sys.exit(1)
来源：http://zpb.redwolf501.top

PHP:  exit(1);
来源：http://gkk.zdqjudy.top

JS:   process.exit(1)
来源：http://nwm.0kj1m.cn

TS:   process.exit(1)
来源：http://kqd.hongshengwenyu.top

Java: System.exit(1)
来源：http://nmh.tanke756.top

Go:   os.Exit(1)
来源：http://vmx.epnwcf.com

Ruby: exit 1
来源：http://tii.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://imh.aizwys.cn

[M06] 向标准错误输出
来源：http://ffb.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://iwo.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://kvp.sysykeji.top

JS:   console.error("err")
来源：http://ork.hnqzz.top

TS:   console.error("err")
来源：http://vht.316326.xyz

Java: System.err.println("err")
来源：http://fsh.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hyp.sufxvd.cn

Ruby: warn "err"
来源：http://tev.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://mcp.chenzaomai.com

[M07] 判断是否为主入口
来源：http://ser.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://zgt.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gll.fengsongda.top

JS:   require.main === module
来源：http://nif.epnwcf.com

TS:   require.main === module
来源：http://pgm.hysaishi.cn

Java: public static void main(String[] args)
来源：http://taj.ydzc1.top

Go:   func main()
来源：http://jcu.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qge.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://gia.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://fem.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://okr.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://uxr.sweek.top

JS:   process.platform;  process.version
来源：http://zon.havefunace.top

TS:   process.platform;  process.version
来源：http://spe.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qmk.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqd.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://exk.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dce.yueranfly.top

================================================================================
来源：http://nxq.shangyingyoupin.top

N. 数据结构与算法
来源：http://vxp.hcnkem.com

================================================================================
来源：http://vgs.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://xpj.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://lfs.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lnw.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqv.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mus.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://coa.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://noc.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pvx.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://njs.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://pwa.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://exv.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ryw.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cer.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zie.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfn.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://wfm.chenlongwang.top

Ruby: arr.sort
来源：http://qce.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ccw.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://kkl.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lrs.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://xsr.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyj.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hde.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tpi.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bya.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sxn.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://nus.dashuyun.cn

[N04] 斐波那契数列
来源：http://qse.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zzm.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lgi.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzn.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pea.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wft.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kit.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://heu.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pca.shangyingyoupin.top

[N05] 最大公约数
来源：http://yru.havefunace.top

Py:   math.gcd(a, b)
来源：http://mxo.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghe.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gsr.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cze.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yrq.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsu.yonumen.top

Ruby: a.gcd(b)
来源：http://bmv.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nmk.pycfn.com

[N06] 判断回文字符串
来源：http://hdw.wangdashe.top

Py:   s == s[::-1]
来源：http://bpp.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://jhv.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://pxx.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://gtq.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jwf.fehbvm.com

Go:   // 双指针从两端比较
来源：http://tdu.bjfxy.top

Ruby: s == s.reverse
来源：http://are.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ekx.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://mlf.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsl.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oen.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wun.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://rlo.shzxlz.cn

Java: // 手写 HashMap
来源：http://uqk.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://tzh.sxryk.cn

Ruby: // 手写 Hash
来源：http://cfa.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bhw.wangdashe.top

[N08] 生成全排列
来源：http://tuf.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://nxi.daxiang520.top

PHP:  // 手写递归交换
来源：http://dmn.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://hrj.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://etg.hnxiangtu.top

Java: // 手写回溯递归
来源：http://wkt.jianghu66.top

Go:   // 手写回溯递归
来源：http://ffj.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://smo.hesvh.cn

C#:   // 手写回溯递归
来源：http://ibe.snrcjt.cn

[N09] 栈与队列
来源：http://mhc.redwolf501.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gvg.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tae.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cqu.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mcd.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eso.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gad.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikv.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://phn.hesvh.cn

[N10] 链表节点定义
来源：http://nmr.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sda.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ttq.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vwc.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qdy.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://ngn.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://rnb.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bzw.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://umk.smart0.xyz

[N11] 二叉树中序遍历
来源：http://flg.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sti.xuanzx.com

PHP:  // 手写递归函数
来源：http://raq.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hte.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpi.fehbvm.com

Java: // 手写递归
来源：http://rnp.yuanzhike.top

Go:   // 手写递归
来源：http://tnq.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ohq.fktsv.cn

C#:   // 手写递归
来源：http://kws.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ryi.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hcs.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uux.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbf.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lsy.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://myn.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wwk.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hjr.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bnq.yvedp.cn

================================================================================
来源：http://kqd.tianlin.xyz

O. 并发与异步
来源：http://nuv.snrcjt.cn

================================================================================
来源：http://qtw.hnqzz.top

[O01] 启动一个线程
来源：http://ylg.bjfxy.top


<!-- 参考信息 -->