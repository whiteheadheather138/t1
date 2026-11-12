代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://lim.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://glw.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uwl.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://xxm.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://zdd.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tav.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xxm.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdp.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bzb.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxe.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jqm.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qhn.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://myd.xuanzx.com

[K07] 进制转换
来源：http://uau.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pml.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://txu.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pji.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hgv.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lzu.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbl.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ujc.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zxj.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://vuo.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://thf.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://glu.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://oru.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://tpa.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fmb.guannengcc.top

Go:   encoding/gob
来源：http://zbw.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://mwn.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddt.jinyuanbaomall.cn

================================================================================
来源：http://tgo.iojbl.cn

L. 网络请求
来源：http://sam.wangshuangyany.cn

================================================================================
来源：http://ouh.pycfn.com

[L01] 发送 GET 请求
来源：http://ohq.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ypz.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yne.hywenlv.cn

JS:   await fetch(url)
来源：http://tlo.ivvv.top

TS:   await fetch(url)
来源：http://mak.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gow.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://myz.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gzg.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vkf.nanxinkj.top

[L02] 发送 POST JSON
来源：http://fpe.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hdc.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gxa.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fpx.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://euk.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mbw.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yrd.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wir.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kbg.hywenlv.cn

[L03] 设置自定义请求头
来源：http://aul.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tul.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzn.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsc.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dpf.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oup.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bua.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cbr.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://crq.wangshuangyany.cn

[L04] 设置超时
来源：http://gml.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://kma.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vrf.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://exc.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://the.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pyh.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://woh.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zka.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uya.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://wiu.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://smj.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ofg.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwu.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfu.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hae.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxh.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vpu.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ulx.shuidangran.top

[L06] 解析响应为 JSON
来源：http://hug.hnxiangtu.top

Py:   resp.json()
来源：http://ohr.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://jui.feifeiyinyue.top

JS:   await resp.json()
来源：http://umk.yanxiufei.cn

TS:   await resp.json()
来源：http://vcm.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kon.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lqi.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://fkp.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjh.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://jdb.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tmx.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ezz.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://dnd.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://fsz.meibo888.top

Java: resp.statusCode()
来源：http://nrs.birdmap.top

Go:   resp.StatusCode
来源：http://tzd.jiagoushi.top

Ruby: resp.code.to_i
来源：http://byj.tanke756.top

C#:   (int)resp.StatusCode
来源：http://niz.bbcook.cn

[L08] 并发请求多个地址
来源：http://usm.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gwd.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://oaz.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nae.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pry.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gxz.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dbw.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://srl.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nmv.fanxiaobao.xyz

================================================================================
来源：http://lqq.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://jsw.yangfankeji.com

================================================================================
来源：http://cay.dashuyun.cn

[M01] 读取命令行参数
来源：http://ljn.sxryk.cn

Py:   sys.argv[1:]
来源：http://rwy.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://bac.xinyue.icu

JS:   process.argv.slice(2)
来源：http://yeg.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://iov.havefunace.top

Java: args 数组（main 方法参数）
来源：http://tdr.ehwqpu.com

Go:   os.Args[1:]
来源：http://ghl.svipenyu.cn

Ruby: ARGV
来源：http://msd.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://kwg.hnqzz.top

[M02] 读取环境变量
来源：http://oeu.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://xwn.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://doe.chenlongwang.top

JS:   process.env.HOME
来源：http://smr.cdnleiting.top

TS:   process.env.HOME
来源：http://dup.jyoumei.cn

Java: System.getenv("HOME")
来源：http://vhr.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lbf.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://tak.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ffc.bjfxy.top

[M03] 执行外部命令
来源：http://wom.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dop.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://udn.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://giv.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qfu.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ydb.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pfu.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jlq.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://cqo.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://amw.zdbjq.cn

Py:   os.getcwd()
来源：http://pzh.meibo888.top

PHP:  getcwd();
来源：http://six.yonumen.top

JS:   process.cwd()
来源：http://sxw.chenlongwang.top

TS:   process.cwd()
来源：http://nrd.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://inx.haohaochexian.top

Go:   os.Getwd()
来源：http://won.yj20258.top

Ruby: Dir.pwd
来源：http://shq.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://yzc.jyoumei.cn

[M05] 设置退出码
来源：http://joz.9152youxi.cn

Py:   sys.exit(1)
来源：http://xpp.hcnkem.com

PHP:  exit(1);
来源：http://kmq.haohaochexian.top

JS:   process.exit(1)
来源：http://bqf.tarul.cn

TS:   process.exit(1)
来源：http://khe.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://aea.jinqigufen.top

Go:   os.Exit(1)
来源：http://dxo.xuanzx.com

Ruby: exit 1
来源：http://gef.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nug.vehdjk.com

[M06] 向标准错误输出
来源：http://zvi.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://ufn.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zsj.ybcxt.top

JS:   console.error("err")
来源：http://kzw.yfazqb.com

TS:   console.error("err")
来源：http://gkg.sxryk.cn

Java: System.err.println("err")
来源：http://res.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://szn.tarul.cn

Ruby: warn "err"
来源：http://whc.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://mhz.gotoacloud.top

[M07] 判断是否为主入口
来源：http://qhx.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://ksv.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ngn.fzhhl.top

JS:   require.main === module
来源：http://dmg.vehdjk.com

TS:   require.main === module
来源：http://eht.daria6918.cn

Java: public static void main(String[] args)
来源：http://pyf.guowangkeji.top

Go:   func main()
来源：http://evh.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jnr.guannengcc.top

C#:   static void Main(string[] args)
来源：http://axi.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://qol.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://int.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://onm.uphjek.com

JS:   process.platform;  process.version
来源：http://axy.yuxming.cn

TS:   process.platform;  process.version
来源：http://wgb.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oza.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wrz.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://niu.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://szh.guannengcc.top

================================================================================
来源：http://wxa.chenjidiqi.icu

N. 数据结构与算法
来源：http://ifc.cdnleiting.top

================================================================================
来源：http://uyd.cashguo.top

[N01] 二分查找（有序数组）
来源：http://zyp.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://bor.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fpl.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eog.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fnp.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vck.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://dbn.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rui.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://ahm.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://qmv.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://jbz.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hav.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nbe.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hdb.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tnr.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://jbd.smart0.xyz

Ruby: arr.sort
来源：http://hne.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hjb.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://rob.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rmi.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://ngw.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gix.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppk.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hwv.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tti.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nkm.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://sql.meibo888.top

[N04] 斐波那契数列
来源：http://bbq.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uhw.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hub.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hef.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uza.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://grc.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://unm.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nck.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ttj.zhengqikj.top

[N05] 最大公约数
来源：http://hdk.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://izs.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jbz.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcg.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tid.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nhz.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brk.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://xqt.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfw.hysaishi.cn

[N06] 判断回文字符串
来源：http://fef.cqqwz.cn

Py:   s == s[::-1]
来源：http://dwu.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://ifr.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://wef.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://mlh.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bft.daria6918.cn

Go:   // 双指针从两端比较
来源：http://jhx.hnxiangtu.top

Ruby: s == s.reverse
来源：http://waq.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://fme.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://uxn.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://duk.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://duy.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ixs.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://vax.chenlongwang.top

Java: // 手写 HashMap
来源：http://vtw.fengsongda.top

Go:   // 手写 map[int]int
来源：http://qzd.zhengqikj.top

Ruby: // 手写 Hash
来源：http://xxx.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://xhq.mhx1999.top

[N08] 生成全排列
来源：http://lgd.havefunace.top

Py:   itertools.permutations(arr)
来源：http://ehg.bbcook.cn

PHP:  // 手写递归交换
来源：http://uxw.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://ryu.jiagoushi.top

TS:   // 手写回溯递归
来源：http://nen.yj202588.top

Java: // 手写回溯递归
来源：http://pge.dashuyun.cn

Go:   // 手写回溯递归
来源：http://xga.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://shv.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://eqg.vqdsnc.cn

[N09] 栈与队列
来源：http://gbd.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hqe.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vnv.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxf.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fwf.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qps.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gzq.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xhl.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://skl.pengpengdd.cyou

[N10] 链表节点定义
来源：http://iag.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wsr.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bbq.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ode.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ull.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://uls.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://jow.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://olw.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fky.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://udo.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vtq.9152youxi.cn

PHP:  // 手写递归函数
来源：http://koi.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vzt.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dzg.zhengqikj.top

Java: // 手写递归
来源：http://myy.havefunace.top

Go:   // 手写递归
来源：http://fhg.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lim.xuanzx.com

C#:   // 手写递归
来源：http://jbh.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://teh.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wrf.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pef.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ivu.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epx.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajb.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xfu.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zee.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppy.haohaochexian.top

================================================================================
来源：http://sem.jyoumei.cn

O. 并发与异步
来源：http://ikf.bjfxy.top

================================================================================
来源：http://lal.ybcxt.top

[O01] 启动一个线程
来源：http://eoq.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jgd.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rkb.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qod.svipenyu.cn

TS:   // 同 JS
来源：http://bjp.316326.xyz


<!-- 参考信息 -->