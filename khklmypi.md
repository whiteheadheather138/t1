代发 wailian999

TS:   JSON.parse(s)
来源：http://wzp.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tsu.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://xyg.shuidangran.top

Ruby: JSON.parse(s)
来源：http://ids.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mtl.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://tam.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wrz.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gpf.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://rzx.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eeb.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uxh.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fli.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://zrh.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hrw.yuxming.cn

[K04] 读取 JSON 文件
来源：http://swn.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rre.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zwj.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqk.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ong.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ooy.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jjg.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gfi.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mrk.daria6918.cn

[K05] 深拷贝对象
来源：http://hue.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://dut.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://kjn.nanxinkj.top

JS:   structuredClone(obj)
来源：http://ccz.shuidangran.top

TS:   structuredClone(obj)
来源：http://zqg.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ifc.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://smg.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jcd.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ktv.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://uqi.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gsd.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cun.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://igv.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nuc.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://irm.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sup.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iry.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xrg.smart0.xyz

[K07] 进制转换
来源：http://rsn.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mwy.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ncz.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hrd.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dqb.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xlw.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://atu.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uvy.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tqh.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://zdh.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://lmh.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eaw.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://ccb.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://dgd.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://egp.vqdsnc.cn

Go:   encoding/gob
来源：http://cvj.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://lwf.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xch.iojbl.cn

================================================================================
来源：http://clv.kuanghao11.cn

L. 网络请求
来源：http://pxn.zycfv.cn

================================================================================
来源：http://mzu.tian-w.cn

[L01] 发送 GET 请求
来源：http://kuu.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rbp.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vxs.hesvh.cn

JS:   await fetch(url)
来源：http://htc.sjlbkw.cn

TS:   await fetch(url)
来源：http://kac.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kxg.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://gqr.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dmw.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ymt.hfpthk.cn

[L02] 发送 POST JSON
来源：http://fqt.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://vlj.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ltz.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbs.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oah.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpz.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xda.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bva.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tmb.redwolf501.top

[L03] 设置自定义请求头
来源：http://gxp.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dir.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ioc.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zot.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqq.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ojr.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://spx.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hmg.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kgy.tarul.cn

[L04] 设置超时
来源：http://sli.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://jpz.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ryx.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jaq.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vnl.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hxl.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kqx.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hru.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sbz.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://dzf.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qtb.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://idh.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qab.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nla.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iba.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://czz.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ipo.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://egr.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://jts.dashuyun.cn

Py:   resp.json()
来源：http://mkd.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://rbe.tianlin.xyz

JS:   await resp.json()
来源：http://ngd.hysaishi.cn

TS:   await resp.json()
来源：http://gbl.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xmc.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://brw.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://xyg.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xaj.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://mwt.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lvv.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wkn.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://thq.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://ebu.yj20258888.top

Java: resp.statusCode()
来源：http://bnd.smart0.xyz

Go:   resp.StatusCode
来源：http://kvp.yongpay.top

Ruby: resp.code.to_i
来源：http://xre.sweek.top

C#:   (int)resp.StatusCode
来源：http://goi.hywenlv.cn

[L08] 并发请求多个地址
来源：http://qjk.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://std.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://gpe.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jov.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jlt.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sdi.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lbp.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ews.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qap.bjfxy.top

================================================================================
来源：http://lwp.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://tzg.birdmap.top

================================================================================
来源：http://ylb.yuxming.cn

[M01] 读取命令行参数
来源：http://yjb.vehdjk.com

Py:   sys.argv[1:]
来源：http://fzv.sxryk.cn

PHP:  $argv;  $argc;
来源：http://ctt.cheryme.top

JS:   process.argv.slice(2)
来源：http://rgi.cashguo.top

TS:   process.argv.slice(2)
来源：http://wwv.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://xbh.bbcook.cn

Go:   os.Args[1:]
来源：http://diz.feifeiyinyue.top

Ruby: ARGV
来源：http://hsc.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://uzk.fengsongda.top

[M02] 读取环境变量
来源：http://tzf.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://tnq.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xwi.zhoulong.xyz

JS:   process.env.HOME
来源：http://zcd.hnxiangtu.top

TS:   process.env.HOME
来源：http://njo.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://cce.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ird.guannengcc.top

Ruby: ENV["HOME"]
来源：http://jcd.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yzx.yueranfly.top

[M03] 执行外部命令
来源：http://axs.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hth.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcj.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jtj.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dik.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vkp.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qzw.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xjm.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://gyc.cashguo.top

[M04] 获取当前工作目录
来源：http://zzp.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://fuj.mhx1999.top

PHP:  getcwd();
来源：http://ewl.yj20258.top

JS:   process.cwd()
来源：http://fmn.uphjek.com

TS:   process.cwd()
来源：http://hok.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://lif.andypj.xyz

Go:   os.Getwd()
来源：http://tlo.zdqjudy.top

Ruby: Dir.pwd
来源：http://wge.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ril.tianlin.xyz

[M05] 设置退出码
来源：http://fog.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://vjw.ivvv.top

PHP:  exit(1);
来源：http://jjd.ydzc1.top

JS:   process.exit(1)
来源：http://ikf.tarul.cn

TS:   process.exit(1)
来源：http://hie.fktsv.cn

Java: System.exit(1)
来源：http://xsh.aizwys.cn

Go:   os.Exit(1)
来源：http://usu.jinghuilouyu.cn

Ruby: exit 1
来源：http://jnx.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aiu.yuxming.cn

[M06] 向标准错误输出
来源：http://pud.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://dfc.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ahd.yonumen.top

JS:   console.error("err")
来源：http://wzn.snrcjt.cn

TS:   console.error("err")
来源：http://pio.xinyue.icu

Java: System.err.println("err")
来源：http://scp.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mzc.sysykeji.top

Ruby: warn "err"
来源：http://znr.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://bqk.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://kbs.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://hid.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pbv.tarul.cn

JS:   require.main === module
来源：http://bfv.jqgfzy.top

TS:   require.main === module
来源：http://myh.yonumen.top

Java: public static void main(String[] args)
来源：http://jdq.quarkkingdee.top

Go:   func main()
来源：http://nqx.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jmd.fzhhl.top

C#:   static void Main(string[] args)
来源：http://zzi.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://kmf.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://ltk.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://dqd.vehdjk.com

JS:   process.platform;  process.version
来源：http://zkh.zdqjudy.top

TS:   process.platform;  process.version
来源：http://vsk.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gzg.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzw.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xzs.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nnf.jqgufenzy.top

================================================================================
来源：http://htx.zhixingplan.top

N. 数据结构与算法
来源：http://wrt.hongshengwenyu.top

================================================================================
来源：http://mii.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://ucv.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://syc.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://doz.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hst.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xah.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://cne.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://cid.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://psk.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://qwn.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://dvp.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://tlt.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ecy.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dfb.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dam.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xbx.aizwys.cn

Go:   slices.Sort(arr)
来源：http://tmm.yj202588.top

Ruby: arr.sort
来源：http://uph.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://dvq.meibo888.top

[N03] 快速排序（分治示例）
来源：http://quh.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fhm.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://key.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppr.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckk.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ouf.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://imm.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fbn.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://pgg.bbcook.cn

[N04] 斐波那契数列
来源：http://wfa.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://poi.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://spj.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjf.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uad.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ddx.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lta.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://apd.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iir.yongpay.top

[N05] 最大公约数
来源：http://zjr.yueranfly.top

Py:   math.gcd(a, b)
来源：http://hib.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wuo.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jrm.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dam.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wbp.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://muq.xziqi.cn

Ruby: a.gcd(b)
来源：http://eox.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tvo.gzhubu.top

[N06] 判断回文字符串
来源：http://yfm.dashuyun.cn

Py:   s == s[::-1]
来源：http://clm.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://mmd.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://tww.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://nys.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gdt.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://myv.zhoulong.xyz

Ruby: s == s.reverse
来源：http://lwg.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wpr.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://aks.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zhq.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bkv.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qqu.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://enp.bbcook.cn

Java: // 手写 HashMap
来源：http://avc.fktsv.cn

Go:   // 手写 map[int]int
来源：http://mhs.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://lzk.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://bhm.yongpay.top

[N08] 生成全排列
来源：http://exu.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://fml.hesvh.cn

PHP:  // 手写递归交换
来源：http://vbh.yonumen.top

JS:   // 手写回溯递归
来源：http://ltx.gotoacloud.top

TS:   // 手写回溯递归
来源：http://les.cdnleiting.top

Java: // 手写回溯递归
来源：http://dli.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://tkj.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://cjb.zhixingplan.top

C#:   // 手写回溯递归
来源：http://tso.dianchejie.cn

[N09] 栈与队列
来源：http://xze.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vug.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hsw.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bll.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vtp.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vhx.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qcc.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozt.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehu.ehwqpu.com

[N10] 链表节点定义
来源：http://nfw.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ula.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zat.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vit.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://myg.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://ynj.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://hce.sweek.top


<!-- 参考信息 -->