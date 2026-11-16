代发 wailian999

[K06] 解析 URL 查询串
来源：http://dzx.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://smy.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fnx.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxj.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jte.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qqa.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gik.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dis.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xnj.cucudq.cn

[K07] 进制转换
来源：http://zzh.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tye.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://juq.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uoa.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tou.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxe.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wsy.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggu.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mem.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://vjk.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://qnb.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nbm.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://bhg.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://qri.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dvb.yj20258888.top

Go:   encoding/gob
来源：http://lpm.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://msi.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zii.wangdashe.top

================================================================================
来源：http://exw.gogol.net.cn

L. 网络请求
来源：http://nsp.gotoacloud.top

================================================================================
来源：http://pcp.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://wbx.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vjt.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ydy.hfpthk.cn

JS:   await fetch(url)
来源：http://lpd.jqgfzy.top

TS:   await fetch(url)
来源：http://wou.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kez.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://jwl.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kqw.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cpl.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://dvr.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://chg.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hmn.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gwi.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qak.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yoo.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mig.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iwk.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cyr.shzxlz.cn

[L03] 设置自定义请求头
来源：http://eqv.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vnf.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xul.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://api.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lnu.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mhu.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgy.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dmk.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hib.ywan-chungtsiang.top

[L04] 设置超时
来源：http://cvv.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://ash.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gzc.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irg.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ekq.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cxy.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cnf.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mpl.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ete.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://uiy.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yjj.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqs.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sfz.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ahp.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kzu.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://udr.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wua.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bzp.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://zhk.jianghu66.top

Py:   resp.json()
来源：http://jco.hammf.cn

PHP:  json_decode($body, true);
来源：http://pls.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://vxx.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://mwf.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rpw.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ofk.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://lml.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://onm.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://kkw.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://twl.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lri.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://lkt.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://ndf.uphjek.com

Java: resp.statusCode()
来源：http://eyt.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://usg.zhengqikj.top

Ruby: resp.code.to_i
来源：http://cmt.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://yrt.chenlongwang.top

[L08] 并发请求多个地址
来源：http://ojj.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xma.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://uhy.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eag.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pci.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qhm.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://asy.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bee.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://thv.yj202588.top

================================================================================
来源：http://cdx.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://gyj.0kj1m.cn

================================================================================
来源：http://jrf.zhixingplan.top

[M01] 读取命令行参数
来源：http://ksy.tanke756.top

Py:   sys.argv[1:]
来源：http://xhh.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://ura.cucudq.cn

JS:   process.argv.slice(2)
来源：http://bdf.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://mmh.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://ntb.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://ujv.fehbvm.com

Ruby: ARGV
来源：http://twr.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://nww.hongshengwenyu.top

[M02] 读取环境变量
来源：http://wvy.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://pcc.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://byv.snrcjt.cn

JS:   process.env.HOME
来源：http://nut.cucudq.cn

TS:   process.env.HOME
来源：http://ypv.aizwys.cn

Java: System.getenv("HOME")
来源：http://thk.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jsz.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://nqm.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ciu.mhx1999.top

[M03] 执行外部命令
来源：http://ajf.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ryh.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ryu.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tbw.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://smb.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vdl.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://avi.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://ial.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://jfi.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://kwi.9152youxi.cn

Py:   os.getcwd()
来源：http://qyn.guannengcc.top

PHP:  getcwd();
来源：http://sgp.yj20258.top

JS:   process.cwd()
来源：http://oqa.snrcjt.cn

TS:   process.cwd()
来源：http://oqp.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://oai.shzxlz.cn

Go:   os.Getwd()
来源：http://jii.zhoulong.xyz

Ruby: Dir.pwd
来源：http://tdj.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://amz.sufxvd.cn

[M05] 设置退出码
来源：http://jqq.yuxming.cn

Py:   sys.exit(1)
来源：http://ysf.jqgufenzy.top

PHP:  exit(1);
来源：http://puj.yuanzhike.top

JS:   process.exit(1)
来源：http://ngm.hysaishi.cn

TS:   process.exit(1)
来源：http://lci.haohaochexian.top

Java: System.exit(1)
来源：http://kix.dashuyun.cn

Go:   os.Exit(1)
来源：http://hrn.hammf.cn

Ruby: exit 1
来源：http://yqt.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bvr.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://mxt.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://xmb.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kvf.xziqi.cn

JS:   console.error("err")
来源：http://lnn.jlsjyb.cn

TS:   console.error("err")
来源：http://twh.fengsongda.top

Java: System.err.println("err")
来源：http://xyx.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bnu.tarul.cn

Ruby: warn "err"
来源：http://cbg.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://nnz.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://jgb.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://cki.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jkb.nwbrower.top

JS:   require.main === module
来源：http://odp.yvedp.cn

TS:   require.main === module
来源：http://ydp.zycfv.cn

Java: public static void main(String[] args)
来源：http://etx.fzhhl.top

Go:   func main()
来源：http://uht.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rhd.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://eso.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://dal.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://are.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://oqp.tanke756.top

JS:   process.platform;  process.version
来源：http://cya.ehwqpu.com

TS:   process.platform;  process.version
来源：http://qey.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oey.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aex.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://erd.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xyu.yj20258.top

================================================================================
来源：http://wjt.vehdjk.com

N. 数据结构与算法
来源：http://gop.yfazqb.com

================================================================================
来源：http://khq.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://jpv.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://mlq.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xcg.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqp.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://saz.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://dfb.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://kim.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jzt.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://hlq.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://apj.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://bll.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cha.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://opo.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wlr.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://scl.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://bre.gzhubu.top

Ruby: arr.sort
来源：http://lpu.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://blx.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://tei.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vmr.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://dzu.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ewp.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rgt.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rpy.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wqu.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uqg.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://wdm.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://yhg.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dcd.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nnq.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhw.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ajo.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzp.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bvl.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rvc.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mdx.smart0.xyz

[N05] 最大公约数
来源：http://zxk.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://fyo.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bhh.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrz.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npj.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xny.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yzv.hysaishi.cn

Ruby: a.gcd(b)
来源：http://yhm.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pta.svipenyu.cn

[N06] 判断回文字符串
来源：http://hig.sufxvd.cn

Py:   s == s[::-1]
来源：http://act.mhx1999.top

PHP:  $s === strrev($s);
来源：http://jur.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://lzi.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://kwd.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ned.cashguo.top

Go:   // 双指针从两端比较
来源：http://nub.sweek.top

Ruby: s == s.reverse
来源：http://sel.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://orv.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://atd.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ohq.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uig.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://vip.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://cud.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://zcj.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://exp.9152youxi.cn

Ruby: // 手写 Hash
来源：http://jsk.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://nnb.fanxiaobao.xyz

[N08] 生成全排列
来源：http://tow.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://gqp.chenzaomai.com

PHP:  // 手写递归交换
来源：http://vez.ivvv.top

JS:   // 手写回溯递归
来源：http://yuh.ctjpmb.com

TS:   // 手写回溯递归
来源：http://vyn.hnxiangtu.top

Java: // 手写回溯递归
来源：http://lmz.gotoacloud.top

Go:   // 手写回溯递归
来源：http://evs.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://edr.ppjwa.cn

C#:   // 手写回溯递归
来源：http://cru.tianlin.xyz

[N09] 栈与队列
来源：http://tca.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oqj.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bwp.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wbc.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dph.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oso.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cmn.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqz.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wek.tarul.cn

[N10] 链表节点定义
来源：http://bce.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pmf.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pcm.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dcq.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zlc.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://wcb.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://zfk.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tem.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kgw.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://kum.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eue.yj20258.top

PHP:  // 手写递归函数
来源：http://dnv.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iim.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fbf.jqgufenzy.top

Java: // 手写递归
来源：http://avp.daxiang520.top

Go:   // 手写递归
来源：http://wvs.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://agi.jianghu66.top

C#:   // 手写递归
来源：http://qqb.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mpm.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tuu.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fap.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zyz.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fwc.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kqz.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://upu.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gej.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vbo.yj20258888.top

================================================================================
来源：http://nvx.jqgufenzy.top

O. 并发与异步
来源：http://fle.andypj.xyz

================================================================================
来源：http://pwk.yj202588.top

[O01] 启动一个线程
来源：http://zhv.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rbm.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://usp.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jwc.jinqigfzy.top

TS:   // 同 JS
来源：http://vfl.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://bsg.cheryme.top

Go:   go f()
来源：http://efl.hfpthk.cn

Ruby: Thread.new { f }
来源：http://squ.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://zxx.yfazqb.com


<!-- 参考信息 -->