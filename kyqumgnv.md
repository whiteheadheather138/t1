代发 wailian999

[K06] 解析 URL 查询串
来源：http://irv.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nrp.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://azd.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kld.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyr.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kil.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dgj.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oql.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oxq.vqdsnc.cn

[K07] 进制转换
来源：http://hju.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vgy.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kps.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svm.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qhx.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zsx.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rce.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://smt.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sjr.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://qha.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://qjz.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rxy.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://jym.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://jav.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zqy.fanxiaobao.xyz

Go:   encoding/gob
来源：http://nhz.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://adz.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iet.tarul.cn

================================================================================
来源：http://qos.bjfxy.top

L. 网络请求
来源：http://pjd.tarul.cn

================================================================================
来源：http://bvc.cashguo.top

[L01] 发送 GET 请求
来源：http://edc.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eoc.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lkw.bbcook.cn

JS:   await fetch(url)
来源：http://hmn.birdmap.top

TS:   await fetch(url)
来源：http://tyw.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sus.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://ejs.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sje.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yla.zhixingplan.top

[L02] 发送 POST JSON
来源：http://pdr.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://amz.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cns.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxm.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iva.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kib.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mzz.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hfb.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qfj.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://mlb.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lty.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vol.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gez.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bit.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xyg.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jew.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tjt.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ttn.gogol.net.cn

[L04] 设置超时
来源：http://hms.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://grq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mkc.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qxd.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipz.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cbz.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uju.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://prc.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ehl.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://uif.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hzw.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ehr.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hhz.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gdq.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cbn.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zsu.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vby.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://epu.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://pcz.jlsjyb.cn

Py:   resp.json()
来源：http://vqs.fehbvm.com

PHP:  json_decode($body, true);
来源：http://bfa.dianchejie.cn

JS:   await resp.json()
来源：http://ayq.jlsjyb.cn

TS:   await resp.json()
来源：http://zef.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://huk.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gio.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://enc.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xyb.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://qia.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fap.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://imw.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://pxz.havefunace.top

TS:   resp.ok;  resp.status
来源：http://zxi.hfpthk.cn

Java: resp.statusCode()
来源：http://jzg.316326.xyz

Go:   resp.StatusCode
来源：http://ajw.chenzaomai.com

Ruby: resp.code.to_i
来源：http://aqn.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://ghp.daxiang520.top

[L08] 并发请求多个地址
来源：http://ppo.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ikx.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://egb.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wkd.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iby.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ufn.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbz.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xrn.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iib.wangdashe.top

================================================================================
来源：http://zov.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://ant.daria6918.cn

================================================================================
来源：http://wco.tianlin.xyz

[M01] 读取命令行参数
来源：http://xns.zhengqikj.top

Py:   sys.argv[1:]
来源：http://por.hnqzz.top

PHP:  $argv;  $argc;
来源：http://cco.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://fva.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://zmi.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://aww.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://kcy.jinqigfzy.top

Ruby: ARGV
来源：http://laz.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://vpn.zhijiandao.cn

[M02] 读取环境变量
来源：http://fcg.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://ffy.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pgk.aizwys.cn

JS:   process.env.HOME
来源：http://uhj.havefunace.top

TS:   process.env.HOME
来源：http://uzd.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://rxs.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mne.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://irc.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dkk.xuanzx.com

[M03] 执行外部命令
来源：http://pnl.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gpv.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://asi.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uzw.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://qjk.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zfh.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uze.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://jhq.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://sjr.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://vzw.daxiang520.top

Py:   os.getcwd()
来源：http://ofh.hesvh.cn

PHP:  getcwd();
来源：http://ukc.pengpengdd.cyou

JS:   process.cwd()
来源：http://cda.ydjk.org.cn

TS:   process.cwd()
来源：http://vqh.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://bxz.vehdjk.com

Go:   os.Getwd()
来源：http://wej.hcnkem.com

Ruby: Dir.pwd
来源：http://qhk.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://avd.redwolf501.top

[M05] 设置退出码
来源：http://bmo.hywenlv.cn

Py:   sys.exit(1)
来源：http://tcg.gzhubu.top

PHP:  exit(1);
来源：http://yet.chenzaomai.com

JS:   process.exit(1)
来源：http://zck.fktsv.cn

TS:   process.exit(1)
来源：http://gvg.guowangkeji.top

Java: System.exit(1)
来源：http://iih.jyoumei.cn

Go:   os.Exit(1)
来源：http://ibh.nanxuanxn.top

Ruby: exit 1
来源：http://kqw.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cyw.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://rdt.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://wkh.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nxx.yangfankeji.com

JS:   console.error("err")
来源：http://jfj.shangyingyoupin.top

TS:   console.error("err")
来源：http://plg.chenzaomai.com

Java: System.err.println("err")
来源：http://xoh.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogq.xuanzx.com

Ruby: warn "err"
来源：http://suk.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://hwd.fengsongda.top

[M07] 判断是否为主入口
来源：http://bdp.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://wja.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qtj.meibo888.top

JS:   require.main === module
来源：http://ivx.cqqwz.cn

TS:   require.main === module
来源：http://obd.yfazqb.com

Java: public static void main(String[] args)
来源：http://nsh.havefunace.top

Go:   func main()
来源：http://hnh.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hqg.zycfv.cn

C#:   static void Main(string[] args)
来源：http://idy.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://ppz.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://qix.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://jup.tanke756.top

JS:   process.platform;  process.version
来源：http://obl.sxryk.cn

TS:   process.platform;  process.version
来源：http://bzt.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cyo.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wfq.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yhp.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://luz.yongpay.top

================================================================================
来源：http://yse.gogol.net.cn

N. 数据结构与算法
来源：http://wkz.tanke756.top

================================================================================
来源：http://idt.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://pkl.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fdt.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eqp.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://des.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tum.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://ril.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://iha.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwm.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://axm.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://eul.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://cbh.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hdj.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oit.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ftf.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hpb.sysykeji.top

Go:   slices.Sort(arr)
来源：http://vuj.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://uce.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://adr.uphjek.com

[N03] 快速排序（分治示例）
来源：http://urr.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rdb.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://pjn.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zhb.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnz.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zva.yj20258.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wlm.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lys.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://prh.uphjek.com

[N04] 斐波那契数列
来源：http://ooj.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxs.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oys.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lbg.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vap.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wch.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nbq.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cvf.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jfm.chenjidiqi.icu

[N05] 最大公约数
来源：http://vsz.cucudq.cn

Py:   math.gcd(a, b)
来源：http://mac.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qux.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpw.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://efw.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://isu.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pgl.smart0.xyz

Ruby: a.gcd(b)
来源：http://htp.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hmf.zhengqikj.top

[N06] 判断回文字符串
来源：http://cat.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://tyq.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://mlz.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://oqa.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://aty.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fdn.yueranfly.top

Go:   // 双指针从两端比较
来源：http://tbu.uphjek.com

Ruby: s == s.reverse
来源：http://xfg.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lws.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://mqu.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dct.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hzy.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qfm.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://xwz.cqqwz.cn

Java: // 手写 HashMap
来源：http://stx.birdmap.top

Go:   // 手写 map[int]int
来源：http://kbi.haohaochexian.top

Ruby: // 手写 Hash
来源：http://tal.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://ynb.daxiang520.top

[N08] 生成全排列
来源：http://mor.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://tpm.52xcode.cn

PHP:  // 手写递归交换
来源：http://iko.yueranfly.top

JS:   // 手写回溯递归
来源：http://ght.cashguo.top

TS:   // 手写回溯递归
来源：http://hcz.yonumen.top

Java: // 手写回溯递归
来源：http://wwx.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://kqd.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://fzm.hysaishi.cn

C#:   // 手写回溯递归
来源：http://nuj.chenlongwang.top

[N09] 栈与队列
来源：http://gix.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zqi.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sda.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gjo.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qrw.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sls.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vej.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pnj.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://omx.aizwys.cn

[N10] 链表节点定义
来源：http://osl.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rja.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dgm.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hnv.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hpt.sweek.top

Java: class Node { int v; Node next; }
来源：http://ckr.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://tyn.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gzl.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qdg.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://ysk.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qix.sysykeji.top

PHP:  // 手写递归函数
来源：http://tnz.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://toh.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lor.epnwcf.com

Java: // 手写递归
来源：http://oad.ctjpmb.com

Go:   // 手写递归
来源：http://vao.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kqm.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://ayz.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ben.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oes.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kkv.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjt.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tle.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujj.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bsd.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oip.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rse.aibaodan.cn

================================================================================
来源：http://icn.316326.xyz

O. 并发与异步
来源：http://sjy.zhiwuduotai.top

================================================================================
来源：http://jid.shzxlz.cn

[O01] 启动一个线程
来源：http://bzj.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fui.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qob.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xql.jlsjyb.cn

TS:   // 同 JS
来源：http://oym.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://tlu.yj202588.top

Go:   go f()
来源：http://rio.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://aiz.yueranfly.top

C#:   Task.Run(() => F());
来源：http://gkd.nanxuanxn.top


<!-- 参考信息 -->