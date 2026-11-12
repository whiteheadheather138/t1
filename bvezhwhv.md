代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://bvk.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vyx.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://itj.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fpt.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://qqt.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://urw.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://spr.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dte.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://znh.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xit.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ljo.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rap.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zmd.yj202588.top

[K07] 进制转换
来源：http://lvw.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iei.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dhz.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vay.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ecz.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zjp.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rdl.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pqc.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xge.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://kep.yj202588.top

Py:   pickle.dumps(obj)
来源：http://uic.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://exp.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://yvx.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://ejp.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rcr.cheryme.top

Go:   encoding/gob
来源：http://nhz.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://gmz.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ysh.pengpengdd.cyou

================================================================================
来源：http://tpw.shangyingyoupin.top

L. 网络请求
来源：http://fui.meibo888.top

================================================================================
来源：http://iel.nanxinkj.top

[L01] 发送 GET 请求
来源：http://wgs.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zdf.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://atd.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://iwi.shuidangran.top

TS:   await fetch(url)
来源：http://hig.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hzn.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://voh.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://luy.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkt.dianchejie.cn

[L02] 发送 POST JSON
来源：http://dis.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://aea.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oao.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpo.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qev.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vjz.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://arq.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ncv.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iul.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://lko.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gud.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dis.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hbg.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tks.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://foa.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ynj.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fsc.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://roy.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://god.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://suy.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqe.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mqx.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbn.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odf.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://adv.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://auj.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eay.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://xum.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wcf.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ckj.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://juu.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ere.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pph.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xpy.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nef.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gqw.zycfv.cn

[L06] 解析响应为 JSON
来源：http://pgt.meibo888.top

Py:   resp.json()
来源：http://yug.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://wpe.nwbrower.top

JS:   await resp.json()
来源：http://dqe.cdnleiting.top

TS:   await resp.json()
来源：http://olh.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qvb.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mpl.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://abx.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gcs.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://xek.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qzg.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nsi.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://srg.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://fqw.fzhhl.top

Java: resp.statusCode()
来源：http://ykw.hnxiangtu.top

Go:   resp.StatusCode
来源：http://lbc.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://uet.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://avm.yj202588.top

[L08] 并发请求多个地址
来源：http://zdb.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzv.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://ryr.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npv.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qst.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cmc.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wal.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hzz.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ckz.vqdsnc.cn

================================================================================
来源：http://skk.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://lmr.nanxinkj.top

================================================================================
来源：http://ziv.cheryme.top

[M01] 读取命令行参数
来源：http://oyk.guowangkeji.top

Py:   sys.argv[1:]
来源：http://rsh.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://xyq.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://nwj.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://lxj.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://lhk.jqgfzy.top

Go:   os.Args[1:]
来源：http://azj.fktsv.cn

Ruby: ARGV
来源：http://bua.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://uzt.chenlongwang.top

[M02] 读取环境变量
来源：http://ggx.tanke756.top

Py:   os.environ.get("HOME")
来源：http://aya.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rdq.yuxming.cn

JS:   process.env.HOME
来源：http://xqj.sysykeji.top

TS:   process.env.HOME
来源：http://him.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://jau.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://anp.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://vlv.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nge.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://cwh.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tis.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rch.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://svp.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lou.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pbp.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://szx.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://hwq.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://ise.guannengcc.top

[M04] 获取当前工作目录
来源：http://uyq.cheryme.top

Py:   os.getcwd()
来源：http://hbv.pengpengdd.cyou

PHP:  getcwd();
来源：http://uch.jqgfzy.top

JS:   process.cwd()
来源：http://dql.hnqzz.top

TS:   process.cwd()
来源：http://wws.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://ktv.yj20258.top

Go:   os.Getwd()
来源：http://gny.jyoumei.cn

Ruby: Dir.pwd
来源：http://kki.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://ems.gogol.net.cn

[M05] 设置退出码
来源：http://dvf.gaohongyu789.top

Py:   sys.exit(1)
来源：http://ysw.nanxuanxn.top

PHP:  exit(1);
来源：http://fgg.bjfxy.top

JS:   process.exit(1)
来源：http://ued.fktsv.cn

TS:   process.exit(1)
来源：http://zrz.hongshengwenyu.top

Java: System.exit(1)
来源：http://xnk.yongpay.top

Go:   os.Exit(1)
来源：http://qcv.andypj.xyz

Ruby: exit 1
来源：http://wir.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xpg.zycfv.cn

[M06] 向标准错误输出
来源：http://xee.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://wkh.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gak.sjlbkw.cn

JS:   console.error("err")
来源：http://fzc.zhixingplan.top

TS:   console.error("err")
来源：http://vlr.daxiang520.top

Java: System.err.println("err")
来源：http://yck.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tmy.iojbl.cn

Ruby: warn "err"
来源：http://opy.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://hen.cdnleiting.top

[M07] 判断是否为主入口
来源：http://adf.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://zab.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hei.xinyue.icu

JS:   require.main === module
来源：http://eml.zhoulong.xyz

TS:   require.main === module
来源：http://dda.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://zss.gzhubu.top

Go:   func main()
来源：http://dos.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yue.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://hrp.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://qmi.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://ipk.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://mjp.cucudq.cn

JS:   process.platform;  process.version
来源：http://voq.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://qyx.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xny.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qob.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lbl.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oaj.havefunace.top

================================================================================
来源：http://fnv.fzhhl.top

N. 数据结构与算法
来源：http://pgs.sjlbkw.cn

================================================================================
来源：http://kvh.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://lpg.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tya.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kgs.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sve.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofj.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hpl.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://kst.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://khv.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://bql.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://obn.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://suq.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xuv.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwe.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kmi.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://puj.shuidangran.top

Go:   slices.Sort(arr)
来源：http://nxw.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://vdt.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cok.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://abj.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qec.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://ego.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rws.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://emm.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wqy.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://arr.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ksu.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sjp.tanke756.top

[N04] 斐波那契数列
来源：http://qyb.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gfq.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zdt.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jji.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffs.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kvk.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://urs.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hnk.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jqe.gogol.net.cn

[N05] 最大公约数
来源：http://mho.xinyue.icu

Py:   math.gcd(a, b)
来源：http://ywl.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aew.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npw.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kho.zhixingplan.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cev.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ivs.xziqi.cn

Ruby: a.gcd(b)
来源：http://lve.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fkc.hnxiangtu.top

[N06] 判断回文字符串
来源：http://xcq.zhijiandao.cn

Py:   s == s[::-1]
来源：http://yrf.redwolf501.top

PHP:  $s === strrev($s);
来源：http://fvu.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://hhg.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://oxq.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fqz.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://sqq.0kj1m.cn

Ruby: s == s.reverse
来源：http://xuv.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pnt.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://pwe.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://elg.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aiw.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cre.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://qss.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://nza.ydzc1.top

Go:   // 手写 map[int]int
来源：http://sve.hammf.cn

Ruby: // 手写 Hash
来源：http://xln.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://sgv.tian-w.cn

[N08] 生成全排列
来源：http://yja.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://ust.ivvv.top

PHP:  // 手写递归交换
来源：http://cwt.dianchejie.cn

JS:   // 手写回溯递归
来源：http://gfl.fktsv.cn

TS:   // 手写回溯递归
来源：http://mth.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://gqi.yj202588.top

Go:   // 手写回溯递归
来源：http://pys.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://zwp.nwbrower.top

C#:   // 手写回溯递归
来源：http://vww.shangyingyoupin.top

[N09] 栈与队列
来源：http://tjt.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qat.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ywd.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xvm.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hjn.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxm.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ngy.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://moa.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fwt.hammf.cn

[N10] 链表节点定义
来源：http://xzo.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yim.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ukx.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ujt.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lfj.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://mdx.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://ars.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fzl.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://eel.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://yim.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tir.hammf.cn

PHP:  // 手写递归函数
来源：http://gkn.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ppw.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ubm.nwbrower.top

Java: // 手写递归
来源：http://wcr.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://mfb.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://buq.dianchejie.cn

C#:   // 手写递归
来源：http://yxh.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hev.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lvj.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://teo.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqk.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bjz.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nxa.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bjg.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mmm.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kuz.yongpay.top

================================================================================
来源：http://yrq.xinyue.icu

O. 并发与异步
来源：http://zas.fzhhl.top

================================================================================
来源：http://vhw.nanxinkj.top

[O01] 启动一个线程
来源：http://euc.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qpe.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vlw.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gkp.havefunace.top

TS:   // 同 JS
来源：http://myj.bbcook.cn


<!-- 参考信息 -->