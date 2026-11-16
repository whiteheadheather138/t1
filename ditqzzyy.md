代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hyk.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ckg.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhf.hfpthk.cn

[K05] 深拷贝对象
来源：http://kgi.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://rxh.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://nrj.tarul.cn

JS:   structuredClone(obj)
来源：http://cvc.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://gbp.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://plr.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nxt.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uro.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oss.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://fvj.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lmm.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ygl.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cmw.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxa.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gme.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gom.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://viv.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iok.yj20258.top

[K07] 进制转换
来源：http://ctv.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eqz.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ffe.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vjm.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qcp.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyz.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ozp.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wez.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hxc.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://akc.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://ind.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nkg.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://kvs.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://gou.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ifm.zhijiandao.cn

Go:   encoding/gob
来源：http://jdz.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://ief.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nuu.nanxuanxn.top

================================================================================
来源：http://cvx.zhixingplan.top

L. 网络请求
来源：http://cck.gotoacloud.top

================================================================================
来源：http://lti.aibaodan.cn

[L01] 发送 GET 请求
来源：http://ojv.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bca.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zbx.ivvv.top

JS:   await fetch(url)
来源：http://ckv.sweek.top

TS:   await fetch(url)
来源：http://dqx.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yhs.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://arq.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oey.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dja.yueranfly.top

[L02] 发送 POST JSON
来源：http://wmy.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pdo.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wif.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://chl.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eae.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xdd.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hwo.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cce.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ony.andypj.xyz

[L03] 设置自定义请求头
来源：http://qxw.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://orc.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://itv.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lew.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://esw.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lqf.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://avr.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wjq.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://thl.chenzaomai.com

[L04] 设置超时
来源：http://xzz.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://cwi.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://esv.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ery.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bay.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ksi.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://okd.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ewk.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nbg.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://mrv.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yms.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://byb.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vlm.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dnf.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://idq.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tyu.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hml.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uic.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://iew.ehwqpu.com

Py:   resp.json()
来源：http://skf.bjfxy.top

PHP:  json_decode($body, true);
来源：http://zzj.yuanzhike.top

JS:   await resp.json()
来源：http://xhf.ydzc1.top

TS:   await resp.json()
来源：http://ruj.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pwh.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mux.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://hja.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpi.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://kfw.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cqm.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lsu.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://omp.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://pcl.yj20258888.top

Java: resp.statusCode()
来源：http://qni.9152youxi.cn

Go:   resp.StatusCode
来源：http://evv.ctjpmb.com

Ruby: resp.code.to_i
来源：http://tvl.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://ygd.mhx1999.top

[L08] 并发请求多个地址
来源：http://tde.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yxz.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://chw.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lyd.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwq.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dst.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ehg.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fpc.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xpu.nanxuanxn.top

================================================================================
来源：http://phi.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://ywe.gogol.net.cn

================================================================================
来源：http://flp.dianchejie.cn

[M01] 读取命令行参数
来源：http://ioj.gzhubu.top

Py:   sys.argv[1:]
来源：http://eyd.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://xwt.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://wzj.pycfn.com

TS:   process.argv.slice(2)
来源：http://wld.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://qrx.vehdjk.com

Go:   os.Args[1:]
来源：http://nhm.aibaodan.cn

Ruby: ARGV
来源：http://pwr.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://mrl.ppjwa.cn

[M02] 读取环境变量
来源：http://eud.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://rsx.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sfh.tarul.cn

JS:   process.env.HOME
来源：http://diz.hongshengwenyu.top

TS:   process.env.HOME
来源：http://hpm.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://gtk.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yvt.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://esj.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ekn.fengsongda.top

[M03] 执行外部命令
来源：http://mtl.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rwk.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yiz.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qim.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ykh.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgw.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ciq.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://ekd.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://uku.yonumen.top

[M04] 获取当前工作目录
来源：http://shy.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://nvd.fehbvm.com

PHP:  getcwd();
来源：http://aaa.xuanzx.com

JS:   process.cwd()
来源：http://hea.zdbjq.cn

TS:   process.cwd()
来源：http://axy.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://yrf.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://cgw.dashuyun.cn

Ruby: Dir.pwd
来源：http://hss.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vjy.pengpengdd.cyou

[M05] 设置退出码
来源：http://hhl.zdbjq.cn

Py:   sys.exit(1)
来源：http://lwb.yongpay.top

PHP:  exit(1);
来源：http://izk.gogol.net.cn

JS:   process.exit(1)
来源：http://zgq.sxryk.cn

TS:   process.exit(1)
来源：http://ncg.fktsv.cn

Java: System.exit(1)
来源：http://ifr.bbcook.cn

Go:   os.Exit(1)
来源：http://lrc.bjfxy.top

Ruby: exit 1
来源：http://uxf.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qot.jianghu66.top

[M06] 向标准错误输出
来源：http://xnx.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://vny.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://icx.zdqjudy.top

JS:   console.error("err")
来源：http://irm.chenjidiqi.icu

TS:   console.error("err")
来源：http://kdf.hywenlv.cn

Java: System.err.println("err")
来源：http://nwm.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://znk.bbcook.cn

Ruby: warn "err"
来源：http://mel.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://zog.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://yid.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://tff.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tbd.316326.xyz

JS:   require.main === module
来源：http://xls.jyoumei.cn

TS:   require.main === module
来源：http://knm.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://bme.jinghuilouyu.cn

Go:   func main()
来源：http://kss.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://prn.yvedp.cn

C#:   static void Main(string[] args)
来源：http://uos.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://vjp.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://gxt.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://eol.zdbjq.cn

JS:   process.platform;  process.version
来源：http://etp.jianghu66.top

TS:   process.platform;  process.version
来源：http://ztq.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qjz.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rvb.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jqm.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ton.nwbrower.top

================================================================================
来源：http://sdt.daxiang520.top

N. 数据结构与算法
来源：http://zib.nanxinkj.top

================================================================================
来源：http://ajg.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://rqi.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://wzy.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vdf.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fng.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nye.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://qut.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xyf.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qax.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mjh.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://lma.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://qvz.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://six.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tpl.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syf.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bwa.daxiang520.top

Go:   slices.Sort(arr)
来源：http://xob.daxiang520.top

Ruby: arr.sort
来源：http://hxx.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bfh.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://bhs.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sct.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://zuz.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plk.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://biv.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dne.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://obm.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ayb.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gly.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://lgl.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tdb.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cqv.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbp.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iik.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://umb.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vgk.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bik.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cnd.sxryk.cn

[N05] 最大公约数
来源：http://ytu.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://nfp.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://amm.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ccy.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugj.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dfq.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oqq.ehwqpu.com

Ruby: a.gcd(b)
来源：http://kon.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qjc.chenzaomai.com

[N06] 判断回文字符串
来源：http://rar.gogol.net.cn

Py:   s == s[::-1]
来源：http://jlb.vehdjk.com

PHP:  $s === strrev($s);
来源：http://eok.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://brn.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://wsq.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kne.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://yrv.tianlin.xyz

Ruby: s == s.reverse
来源：http://ihk.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://mhc.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://ewz.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://okx.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ars.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://akc.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://hgf.nwbrower.top

Java: // 手写 HashMap
来源：http://loq.daxiang520.top

Go:   // 手写 map[int]int
来源：http://jku.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://mjd.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://sez.shzxlz.cn

[N08] 生成全排列
来源：http://rej.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://mvq.smart0.xyz

PHP:  // 手写递归交换
来源：http://ddy.yuxming.cn

JS:   // 手写回溯递归
来源：http://ezm.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://qdx.ydzc1.top

Java: // 手写回溯递归
来源：http://zoe.c1oappe.top

Go:   // 手写回溯递归
来源：http://zln.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://ojk.gzhubu.top

C#:   // 手写回溯递归
来源：http://ahz.cucudq.cn

[N09] 栈与队列
来源：http://epn.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hsj.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kwx.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jpq.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lop.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bnq.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qrr.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://alb.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uvd.yonumen.top

[N10] 链表节点定义
来源：http://hdq.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fob.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wrx.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pkw.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lkp.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://lqk.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://etp.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://knm.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sxc.hcnkem.com

[N11] 二叉树中序遍历
来源：http://igc.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mrr.redwolf501.top

PHP:  // 手写递归函数
来源：http://xdp.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ewg.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ylc.jlsjyb.cn

Java: // 手写递归
来源：http://mle.fehbvm.com

Go:   // 手写递归
来源：http://zbc.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vps.zhijiandao.cn

C#:   // 手写递归
来源：http://zer.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://prv.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opj.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llo.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rcs.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qer.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fvd.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cpd.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bbw.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xcr.hcnkem.com


<!-- 参考信息 -->