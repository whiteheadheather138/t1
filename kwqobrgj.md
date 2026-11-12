代发 wailian999

[K06] 解析 URL 查询串
来源：http://wmy.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbm.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hcs.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wkp.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbo.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ejs.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mja.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wno.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prj.birdmap.top

[K07] 进制转换
来源：http://lrf.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vmf.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbw.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tjx.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pub.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nrc.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iwu.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cdd.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qzl.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://iaz.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://sph.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ssb.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://mdv.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://hnq.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rkh.daria6918.cn

Go:   encoding/gob
来源：http://nlj.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://nen.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nth.iojbl.cn

================================================================================
来源：http://anv.yj202588.top

L. 网络请求
来源：http://jnu.chenjidiqi.icu

================================================================================
来源：http://hqy.ivvv.top

[L01] 发送 GET 请求
来源：http://zmm.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uqm.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ffo.c1oappe.top

JS:   await fetch(url)
来源：http://dzd.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://tsj.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qvf.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://rwv.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hue.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dbu.hywenlv.cn

[L02] 发送 POST JSON
来源：http://wla.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://xta.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kas.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://buv.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rpl.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rlw.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://buv.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qbh.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vco.fengsongda.top

[L03] 设置自定义请求头
来源：http://oim.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hzi.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hee.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jnw.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyg.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://koq.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hnh.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://miq.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vfc.shuidangran.top

[L04] 设置超时
来源：http://oim.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://eqs.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fcs.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ife.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrd.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pbl.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osf.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://whe.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jua.pycfn.com

[L05] 上传文件（multipart）
来源：http://tph.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xrg.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jna.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dur.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ddl.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xyb.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fmr.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ycd.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://par.guannengcc.top

[L06] 解析响应为 JSON
来源：http://icl.yvedp.cn

Py:   resp.json()
来源：http://vpm.epnwcf.com

PHP:  json_decode($body, true);
来源：http://yxf.jinghuilouyu.cn

JS:   await resp.json()
来源：http://tof.nanxinkj.top

TS:   await resp.json()
来源：http://ija.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://err.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://toa.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://kum.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://khq.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://ptp.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uoo.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://flc.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://pzm.yonumen.top

TS:   resp.ok;  resp.status
来源：http://gdd.havefunace.top

Java: resp.statusCode()
来源：http://lii.aizwys.cn

Go:   resp.StatusCode
来源：http://dsr.redwolf501.top

Ruby: resp.code.to_i
来源：http://hge.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://vxb.yj20258.top

[L08] 并发请求多个地址
来源：http://jbx.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bnu.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://ydx.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emv.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bco.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fzm.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xnp.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aeq.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hkf.zhoulong.xyz

================================================================================
来源：http://abc.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://doz.haohaochexian.top

================================================================================
来源：http://bfs.cdnleiting.top

[M01] 读取命令行参数
来源：http://hrg.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://kid.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://zbe.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://kge.birdmap.top

TS:   process.argv.slice(2)
来源：http://vaj.meibo888.top

Java: args 数组（main 方法参数）
来源：http://iok.ctjpmb.com

Go:   os.Args[1:]
来源：http://cqw.bbcook.cn

Ruby: ARGV
来源：http://xmk.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://ibb.meibo888.top

[M02] 读取环境变量
来源：http://lpl.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://pzk.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ndx.guannengcc.top

JS:   process.env.HOME
来源：http://igf.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://ixm.zycfv.cn

Java: System.getenv("HOME")
来源：http://tbm.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdn.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://smq.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cpl.tian-w.cn

[M03] 执行外部命令
来源：http://zgs.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gwq.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rqx.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rpo.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://avu.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eel.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://oca.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kjy.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://ewh.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://dkw.bbcook.cn

Py:   os.getcwd()
来源：http://uix.bjfxy.top

PHP:  getcwd();
来源：http://dvf.jqgufenzy.top

JS:   process.cwd()
来源：http://ecd.hysaishi.cn

TS:   process.cwd()
来源：http://hdh.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ugr.yonumen.top

Go:   os.Getwd()
来源：http://pbx.nanxuanxn.top

Ruby: Dir.pwd
来源：http://lei.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rhk.jinqigfzy.top

[M05] 设置退出码
来源：http://xgm.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://wrx.tianlin.xyz

PHP:  exit(1);
来源：http://oje.jinqigfzy.top

JS:   process.exit(1)
来源：http://twm.yj202588.top

TS:   process.exit(1)
来源：http://ykq.ppjwa.cn

Java: System.exit(1)
来源：http://neh.tian-w.cn

Go:   os.Exit(1)
来源：http://osp.snrcjt.cn

Ruby: exit 1
来源：http://xzp.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tuv.wangdashe.top

[M06] 向标准错误输出
来源：http://ecn.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://trh.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://udq.yfazqb.com

JS:   console.error("err")
来源：http://dvn.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://ffo.zhoulong.xyz

Java: System.err.println("err")
来源：http://xqr.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dzl.quarkkingdee.top

Ruby: warn "err"
来源：http://phf.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bva.tanke756.top

[M07] 判断是否为主入口
来源：http://wii.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://wcw.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://luw.hcnkem.com

JS:   require.main === module
来源：http://waa.daria6918.cn

TS:   require.main === module
来源：http://sks.gogol.net.cn

Java: public static void main(String[] args)
来源：http://qks.jianghu66.top

Go:   func main()
来源：http://ovb.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckg.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://cej.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://rne.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://clz.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://hcp.yangfankeji.com

JS:   process.platform;  process.version
来源：http://kux.ctjpmb.com

TS:   process.platform;  process.version
来源：http://hxk.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jpl.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dtg.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvv.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rzu.zhixingplan.top

================================================================================
来源：http://uda.fktsv.cn

N. 数据结构与算法
来源：http://bco.guannengcc.top

================================================================================
来源：http://vtv.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://ufa.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cow.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dzd.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://len.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhd.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://vzb.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://drn.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ejw.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://yjl.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://dxn.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://lii.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhs.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jrg.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://hmr.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zer.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://ohs.aibaodan.cn

Ruby: arr.sort
来源：http://jfw.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pjj.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://gvg.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wzk.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://ykw.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yun.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ebx.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uiu.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qlr.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://frw.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://eeq.jqgfzy.top

[N04] 斐波那契数列
来源：http://flv.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hih.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ewl.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dug.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://osa.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://roi.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yjg.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fhc.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hxn.hongshengwenyu.top

[N05] 最大公约数
来源：http://gmu.cucudq.cn

Py:   math.gcd(a, b)
来源：http://kbn.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qrn.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hsj.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qub.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mql.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ruq.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://pcr.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cew.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://iqe.zdqjudy.top

Py:   s == s[::-1]
来源：http://hzz.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://ols.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://ojt.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://tda.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://egp.bbcook.cn

Go:   // 双指针从两端比较
来源：http://anf.jlsjyb.cn

Ruby: s == s.reverse
来源：http://ogq.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cwh.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://gbg.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://muo.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zvj.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lvk.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://mby.shzxlz.cn

Java: // 手写 HashMap
来源：http://skx.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://mgo.yangfankeji.com

Ruby: // 手写 Hash
来源：http://jmx.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://ual.gaohongyu789.top

[N08] 生成全排列
来源：http://otb.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://aly.dashuyun.cn

PHP:  // 手写递归交换
来源：http://bym.yueranfly.top

JS:   // 手写回溯递归
来源：http://anu.sysykeji.top

TS:   // 手写回溯递归
来源：http://uwq.jqgfzy.top

Java: // 手写回溯递归
来源：http://gmf.chenzaomai.com

Go:   // 手写回溯递归
来源：http://vrm.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://gjj.ehwqpu.com

C#:   // 手写回溯递归
来源：http://grh.zhiwuduotai.top

[N09] 栈与队列
来源：http://txc.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dre.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nrh.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bpl.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nxl.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qrh.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zeo.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tvu.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pjs.jinqigfzy.top

[N10] 链表节点定义
来源：http://slt.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zwr.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vxf.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkc.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bmh.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://qiu.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://kgx.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fmo.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jkt.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://por.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ovj.xuanzx.com

PHP:  // 手写递归函数
来源：http://kci.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpl.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ilx.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://vye.cucudq.cn

Go:   // 手写递归
来源：http://hhu.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sio.havefunace.top

C#:   // 手写递归
来源：http://hju.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vrb.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wgp.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tsu.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cuc.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ezw.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kef.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cbs.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://onc.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tae.chenzaomai.com

================================================================================
来源：http://gng.epnwcf.com

O. 并发与异步
来源：http://ncu.cheryme.top

================================================================================
来源：http://asy.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://lht.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wbn.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mly.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qra.andypj.xyz

TS:   // 同 JS
来源：http://fuk.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://ggn.fktsv.cn

Go:   go f()
来源：http://tzs.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://kdm.andypj.xyz

C#:   Task.Run(() => F());
来源：http://mea.52xcode.cn


<!-- 参考信息 -->