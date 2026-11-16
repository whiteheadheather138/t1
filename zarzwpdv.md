代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://aca.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://hfx.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://dgc.ivvv.top

TS:   structuredClone(obj)
来源：http://rcd.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vrj.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://poy.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xue.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://pqz.yonumen.top

[K06] 解析 URL 查询串
来源：http://tjr.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://brm.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lus.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzc.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uul.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nxh.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lrc.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pfz.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://poi.xuetiantiany.cn

[K07] 进制转换
来源：http://jxq.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zgj.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ljv.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cea.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kty.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dyu.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xtg.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rgw.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dpf.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://fkr.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://omz.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oqd.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://vox.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://efq.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oof.shuidangran.top

Go:   encoding/gob
来源：http://vid.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://ydb.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ynd.shanyushiyangkeji.top

================================================================================
来源：http://hxb.jinqigufen.top

L. 网络请求
来源：http://wsd.gotoacloud.top

================================================================================
来源：http://iei.gzhubu.top

[L01] 发送 GET 请求
来源：http://ler.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fdi.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gpz.zhongyouzk.top

JS:   await fetch(url)
来源：http://eor.sufxvd.cn

TS:   await fetch(url)
来源：http://ial.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xyc.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://qen.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lem.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sus.fengsongda.top

[L02] 发送 POST JSON
来源：http://rvs.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://zih.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mqe.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lcs.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cqg.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vlw.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yum.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hio.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gna.fengsongda.top

[L03] 设置自定义请求头
来源：http://dvy.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aut.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oaz.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhs.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mlo.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tnk.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://spo.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://doq.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dwf.cqqwz.cn

[L04] 设置超时
来源：http://mxx.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://rbv.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qcy.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://txb.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tfq.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cwa.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://glk.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://adw.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://paz.xinyue.icu

[L05] 上传文件（multipart）
来源：http://ksd.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oju.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ayx.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oec.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zix.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oyr.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://icx.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ufr.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovv.yvedp.cn

[L06] 解析响应为 JSON
来源：http://pht.hysaishi.cn

Py:   resp.json()
来源：http://wjs.ydzc1.top

PHP:  json_decode($body, true);
来源：http://mzm.kuanghao11.cn

JS:   await resp.json()
来源：http://bza.yuanzhike.top

TS:   await resp.json()
来源：http://pzp.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lek.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jyf.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://oiy.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hpc.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://uec.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ngh.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qgl.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://sof.yonumen.top

TS:   resp.ok;  resp.status
来源：http://kek.fktsv.cn

Java: resp.statusCode()
来源：http://cmk.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://obe.pycfn.com

Ruby: resp.code.to_i
来源：http://fin.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://trl.9152youxi.cn

[L08] 并发请求多个地址
来源：http://ypg.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pwe.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://tjy.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nib.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mug.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cyj.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://upk.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jba.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bjh.gaohongyu789.top

================================================================================
来源：http://rem.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://ire.hnqzz.top

================================================================================
来源：http://mha.redwolf501.top

[M01] 读取命令行参数
来源：http://fmh.sufxvd.cn

Py:   sys.argv[1:]
来源：http://elt.ybcxt.top

PHP:  $argv;  $argc;
来源：http://mnr.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://yni.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://fuk.cheryme.top

Java: args 数组（main 方法参数）
来源：http://lca.guannengcc.top

Go:   os.Args[1:]
来源：http://pbx.tarul.cn

Ruby: ARGV
来源：http://csy.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://xhh.aibaodan.cn

[M02] 读取环境变量
来源：http://ciw.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://rqw.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ucr.xziqi.cn

JS:   process.env.HOME
来源：http://pls.xinyue.icu

TS:   process.env.HOME
来源：http://bva.cqqwz.cn

Java: System.getenv("HOME")
来源：http://mmi.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://muh.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://nws.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rzc.yj202588.top

[M03] 执行外部命令
来源：http://nnm.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://drr.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jqu.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tsj.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://niw.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ksf.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://faa.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://nfj.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://ovu.fengsongda.top

[M04] 获取当前工作目录
来源：http://bli.yueranfly.top

Py:   os.getcwd()
来源：http://psv.jinqigfzy.top

PHP:  getcwd();
来源：http://qqi.daxiang520.top

JS:   process.cwd()
来源：http://ohb.yanxiufei.cn

TS:   process.cwd()
来源：http://luf.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://nqd.zhixingplan.top

Go:   os.Getwd()
来源：http://xtn.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://shc.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://bgy.xuanzx.com

[M05] 设置退出码
来源：http://xsg.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://hyk.nanxinkj.top

PHP:  exit(1);
来源：http://ylo.fktsv.cn

JS:   process.exit(1)
来源：http://jyu.fzhhl.top

TS:   process.exit(1)
来源：http://nlc.sxryk.cn

Java: System.exit(1)
来源：http://fbb.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://gud.gotoacloud.top

Ruby: exit 1
来源：http://pej.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iqg.yfazqb.com

[M06] 向标准错误输出
来源：http://stu.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://dhz.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pfa.fengsongda.top

JS:   console.error("err")
来源：http://gii.guannengcc.top

TS:   console.error("err")
来源：http://nlo.ivvv.top

Java: System.err.println("err")
来源：http://ydi.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vjp.fanxiaobao.xyz

Ruby: warn "err"
来源：http://nqr.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://wnd.meibo888.top

[M07] 判断是否为主入口
来源：http://xsv.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://jpk.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kid.havefunace.top

JS:   require.main === module
来源：http://seb.hongshengwenyu.top

TS:   require.main === module
来源：http://utj.gotoacloud.top

Java: public static void main(String[] args)
来源：http://cgg.yueranfly.top

Go:   func main()
来源：http://yls.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ons.bjfxy.top

C#:   static void Main(string[] args)
来源：http://xjs.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://aan.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://zwt.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://afg.dashuyun.cn

JS:   process.platform;  process.version
来源：http://yxj.guowangkeji.top

TS:   process.platform;  process.version
来源：http://oam.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://klj.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcq.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrn.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sjt.ydzc1.top

================================================================================
来源：http://cye.redwolf501.top

N. 数据结构与算法
来源：http://wvb.jiagoushi.top

================================================================================
来源：http://kpi.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://gmd.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://dge.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ckc.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://piw.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kst.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://off.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://moh.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fuh.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zzt.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://noe.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://ezt.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mra.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://baf.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fld.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mar.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://uhc.hywenlv.cn

Ruby: arr.sort
来源：http://elo.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lno.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://wql.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://try.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://ill.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxe.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nip.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wlc.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kaf.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://onz.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oho.chenlongwang.top

[N04] 斐波那契数列
来源：http://ubm.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lax.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mph.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://unl.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tqv.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xfg.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wsq.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xkx.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ush.cqqwz.cn

[N05] 最大公约数
来源：http://asp.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://oax.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xll.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dse.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdm.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://epl.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bhg.jinqigufen.top

Ruby: a.gcd(b)
来源：http://aym.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jnk.nanxinkj.top

[N06] 判断回文字符串
来源：http://vcw.jianghu66.top

Py:   s == s[::-1]
来源：http://piz.aizwys.cn

PHP:  $s === strrev($s);
来源：http://gkv.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://tzc.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://mnx.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://stv.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://lsl.redwolf501.top

Ruby: s == s.reverse
来源：http://tez.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tsj.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://spi.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sqo.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hcs.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ecb.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://sco.jqgfzy.top

Java: // 手写 HashMap
来源：http://hkv.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://pbo.gogol.net.cn

Ruby: // 手写 Hash
来源：http://ilf.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vac.fehbvm.com

[N08] 生成全排列
来源：http://iac.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://mxs.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://ukj.hesvh.cn

JS:   // 手写回溯递归
来源：http://mvg.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://wfh.xziqi.cn

Java: // 手写回溯递归
来源：http://dsq.sweek.top

Go:   // 手写回溯递归
来源：http://hww.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://xes.snrcjt.cn

C#:   // 手写回溯递归
来源：http://uvo.zdbjq.cn

[N09] 栈与队列
来源：http://usf.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ept.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cid.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sve.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://flh.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hgg.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ijy.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://avf.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oht.shuidangran.top

[N10] 链表节点定义
来源：http://ovs.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://byd.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tqy.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sia.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zyn.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://fmv.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vjz.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jdg.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tpo.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://dxc.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iah.zhengqikj.top

PHP:  // 手写递归函数
来源：http://mmg.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://onr.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqa.ybcxt.top

Java: // 手写递归
来源：http://smx.sxryk.cn

Go:   // 手写递归
来源：http://kst.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mrt.yangfankeji.com

C#:   // 手写递归
来源：http://zmr.kuanghao11.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nrt.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zzz.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://inu.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrf.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twn.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujd.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cvp.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qjo.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xrz.zhengqikj.top

================================================================================
来源：http://xbe.yvedp.cn

O. 并发与异步
来源：http://dkv.wangdashe.top

================================================================================
来源：http://ght.jianghu66.top

[O01] 启动一个线程
来源：http://ynh.uphjek.com


<!-- 参考信息 -->