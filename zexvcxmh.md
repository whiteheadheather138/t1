代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://xsi.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aod.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kgk.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://utb.yj202588.top

[K06] 解析 URL 查询串
来源：http://nef.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vjv.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://abs.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sve.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hkv.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gka.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mee.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lnj.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jkd.daria6918.cn

[K07] 进制转换
来源：http://ugk.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vot.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzw.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ahy.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unc.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hut.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jrp.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oqi.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jbz.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://tji.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://pis.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://muy.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://poq.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://kst.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://faw.ivvv.top

Go:   encoding/gob
来源：http://twi.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://gyi.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ayx.chenjidiqi.icu

================================================================================
来源：http://nwc.yangfankeji.com

L. 网络请求
来源：http://pbn.yanxiufei.cn

================================================================================
来源：http://jff.vehdjk.com

[L01] 发送 GET 请求
来源：http://rxg.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jnm.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cub.vqdsnc.cn

JS:   await fetch(url)
来源：http://gqp.haohaochexian.top

TS:   await fetch(url)
来源：http://vku.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://onb.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://sdp.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xvd.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aiu.hysaishi.cn

[L02] 发送 POST JSON
来源：http://rbv.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vqm.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gmu.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tpc.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvf.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nvx.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://edr.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vup.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lvv.iojbl.cn

[L03] 设置自定义请求头
来源：http://eee.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uek.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://stv.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://obq.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://koc.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zco.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ere.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lpa.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iks.hysaishi.cn

[L04] 设置超时
来源：http://zvp.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://nhe.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://myy.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vht.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phw.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ipb.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hzq.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bsu.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsv.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://jpd.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kih.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://byj.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkl.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ksd.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nyc.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zkl.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vam.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ams.tanke756.top

[L06] 解析响应为 JSON
来源：http://xwm.wangdashe.top

Py:   resp.json()
来源：http://zfn.aizwys.cn

PHP:  json_decode($body, true);
来源：http://fsp.jyoumei.cn

JS:   await resp.json()
来源：http://pxn.andypj.xyz

TS:   await resp.json()
来源：http://wtj.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lzl.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qdv.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://dgl.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yrh.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://wnb.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://myz.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wwr.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://cvm.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://wtr.jqgufenzy.top

Java: resp.statusCode()
来源：http://qak.shuidangran.top

Go:   resp.StatusCode
来源：http://quk.havefunace.top

Ruby: resp.code.to_i
来源：http://fzq.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://tpy.fengsongda.top

[L08] 并发请求多个地址
来源：http://noz.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gzy.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://dot.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://upc.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ami.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lar.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rwp.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fur.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://owd.vqdsnc.cn

================================================================================
来源：http://oey.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://djp.redwolf501.top

================================================================================
来源：http://ary.sjlbkw.cn

[M01] 读取命令行参数
来源：http://bui.xziqi.cn

Py:   sys.argv[1:]
来源：http://alj.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://jem.iojbl.cn

JS:   process.argv.slice(2)
来源：http://eft.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://ghf.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://jqo.yvedp.cn

Go:   os.Args[1:]
来源：http://dpe.kuanghao11.cn

Ruby: ARGV
来源：http://xrw.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://vzn.vehdjk.com

[M02] 读取环境变量
来源：http://tcd.uphjek.com

Py:   os.environ.get("HOME")
来源：http://sav.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://flz.ybcxt.top

JS:   process.env.HOME
来源：http://pbb.zhoulong.xyz

TS:   process.env.HOME
来源：http://nha.daria6918.cn

Java: System.getenv("HOME")
来源：http://fxy.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eqo.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://bfz.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xxq.yueranfly.top

[M03] 执行外部命令
来源：http://aqf.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://txv.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://utv.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://phh.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ikh.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vtp.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nvo.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tjd.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://mxf.sweek.top

[M04] 获取当前工作目录
来源：http://bii.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://tbu.cdnleiting.top

PHP:  getcwd();
来源：http://iwf.yongpay.top

JS:   process.cwd()
来源：http://uxo.cdnleiting.top

TS:   process.cwd()
来源：http://xfo.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://gmf.ehwqpu.com

Go:   os.Getwd()
来源：http://ulp.andypj.xyz

Ruby: Dir.pwd
来源：http://dae.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://emg.svipenyu.cn

[M05] 设置退出码
来源：http://dgx.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://llc.havefunace.top

PHP:  exit(1);
来源：http://kss.guannengcc.top

JS:   process.exit(1)
来源：http://lbh.yj20258888.top

TS:   process.exit(1)
来源：http://xnt.ydjk.org.cn

Java: System.exit(1)
来源：http://czr.9152youxi.cn

Go:   os.Exit(1)
来源：http://iua.yj20258.top

Ruby: exit 1
来源：http://sza.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uyg.hnxiangtu.top

[M06] 向标准错误输出
来源：http://wbv.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://hic.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vtj.cucudq.cn

JS:   console.error("err")
来源：http://usq.jlsjyb.cn

TS:   console.error("err")
来源：http://dzc.daria6918.cn

Java: System.err.println("err")
来源：http://nnx.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rjp.yfazqb.com

Ruby: warn "err"
来源：http://xtb.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://ijx.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://fca.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://irg.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jyi.tanke756.top

JS:   require.main === module
来源：http://era.andypj.xyz

TS:   require.main === module
来源：http://doz.tian-w.cn

Java: public static void main(String[] args)
来源：http://ubf.jlsjyb.cn

Go:   func main()
来源：http://urf.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ycr.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://pzp.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://fga.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://vjs.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://ptq.yuxming.cn

JS:   process.platform;  process.version
来源：http://waq.fengsongda.top

TS:   process.platform;  process.version
来源：http://ecm.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://chx.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rkm.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gwc.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ywc.shangyingyoupin.top

================================================================================
来源：http://pfp.jinqigufen.top

N. 数据结构与算法
来源：http://byv.xinyue.icu

================================================================================
来源：http://ylu.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://qvb.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://xkw.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ozv.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpq.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vha.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fkz.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://eam.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hod.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://kcz.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://skl.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://nuv.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ams.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cuj.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://grz.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qfa.yueranfly.top

Go:   slices.Sort(arr)
来源：http://ymj.gotoacloud.top

Ruby: arr.sort
来源：http://llc.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ixg.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://plc.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wof.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://ppv.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ssc.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rje.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vru.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uou.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dob.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://hak.xinyue.icu

[N04] 斐波那契数列
来源：http://bxx.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xud.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rqt.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ixc.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ouu.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sak.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ofs.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lln.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vtg.tarul.cn

[N05] 最大公约数
来源：http://bqs.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ost.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dtq.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldi.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dft.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itc.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aqx.ppjwa.cn

Ruby: a.gcd(b)
来源：http://oja.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jms.zhongyouzk.top

[N06] 判断回文字符串
来源：http://ege.zycfv.cn

Py:   s == s[::-1]
来源：http://atr.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://qxs.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://ndl.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://wxc.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ctm.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://eea.iojbl.cn

Ruby: s == s.reverse
来源：http://scd.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uey.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://akw.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://btj.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dzj.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://drm.sweek.top

TS:   // 手写 Map<string, number>
来源：http://fcn.hesvh.cn

Java: // 手写 HashMap
来源：http://dwz.yvedp.cn

Go:   // 手写 map[int]int
来源：http://ttg.andypj.xyz

Ruby: // 手写 Hash
来源：http://kpz.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://umk.jqgfzy.top

[N08] 生成全排列
来源：http://tbc.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://jgj.hesvh.cn

PHP:  // 手写递归交换
来源：http://wxh.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://kdx.yuanzhike.top

TS:   // 手写回溯递归
来源：http://smk.gogol.net.cn

Java: // 手写回溯递归
来源：http://ucq.sysykeji.top

Go:   // 手写回溯递归
来源：http://tpb.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://kla.sxryk.cn

C#:   // 手写回溯递归
来源：http://jpv.316326.xyz

[N09] 栈与队列
来源：http://gky.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fxf.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zfz.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mqw.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ctt.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mnh.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gml.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lek.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sqt.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://woq.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lka.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uio.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tzm.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nif.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://igw.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oxs.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qtr.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mfx.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://lra.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pjm.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://kin.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zju.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://whn.c1oappe.top

Java: // 手写递归
来源：http://dpw.9152youxi.cn

Go:   // 手写递归
来源：http://bjl.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdk.pycfn.com

C#:   // 手写递归
来源：http://jpt.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hkc.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nfa.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qap.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uay.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jih.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://znh.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bhh.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://axy.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pqe.guannengcc.top

================================================================================
来源：http://qql.hesvh.cn

O. 并发与异步
来源：http://ybm.uphjek.com

================================================================================
来源：http://svx.sysykeji.top

[O01] 启动一个线程
来源：http://ufq.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bif.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kpy.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qmi.hesvh.cn

TS:   // 同 JS
来源：http://ylz.c1oappe.top


<!-- 参考信息 -->