代发 wailian999

TS:   JSON.parse(s)
来源：http://wom.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sis.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pxm.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://lmh.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ism.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://mqc.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://asp.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hcj.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bdn.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tdu.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oum.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://png.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nea.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ynl.vehdjk.com

[K04] 读取 JSON 文件
来源：http://hne.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txf.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hnp.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mdv.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsz.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kpx.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbp.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ngi.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jfn.yvedp.cn

[K05] 深拷贝对象
来源：http://xvb.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://rew.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://rla.yj20258888.top

JS:   structuredClone(obj)
来源：http://teo.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://iac.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://xzz.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xno.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rxf.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hcp.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://jsc.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jlj.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dhz.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wup.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xni.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjz.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rek.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tog.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ijt.jinqigfzy.top

[K07] 进制转换
来源：http://lyv.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gze.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://val.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jim.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://drn.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uip.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://shx.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://olr.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://plo.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://suy.uphjek.com

Py:   pickle.dumps(obj)
来源：http://bur.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dcu.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://lww.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ylg.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://guo.jqgfzy.top

Go:   encoding/gob
来源：http://zie.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://mnd.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rda.zhoulong.xyz

================================================================================
来源：http://sur.iojbl.cn

L. 网络请求
来源：http://dbr.bbcook.cn

================================================================================
来源：http://kcs.9152youxi.cn

[L01] 发送 GET 请求
来源：http://unp.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wnz.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://flp.nanxinkj.top

JS:   await fetch(url)
来源：http://jdt.zhongyouzk.top

TS:   await fetch(url)
来源：http://igq.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fyy.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://ylv.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dhp.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nyu.cdnleiting.top

[L02] 发送 POST JSON
来源：http://kad.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://bat.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://axx.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hnj.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpq.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rov.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ktz.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oth.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xxo.birdmap.top

[L03] 设置自定义请求头
来源：http://dve.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ddb.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iff.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qbd.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ivm.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ejz.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://upx.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hoe.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bnb.tian-w.cn

[L04] 设置超时
来源：http://yuz.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://fau.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qpb.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pia.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wlu.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ijs.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://brz.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fqy.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jrc.redwolf501.top

[L05] 上传文件（multipart）
来源：http://mns.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sqi.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hhc.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ffi.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qng.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ion.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kwg.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ibw.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vos.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://dlh.zhoulong.xyz

Py:   resp.json()
来源：http://ptx.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://kfn.andypj.xyz

JS:   await resp.json()
来源：http://fzz.andypj.xyz

TS:   await resp.json()
来源：http://ojl.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hmv.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yxc.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://hrj.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qis.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://ixi.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ujb.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zpw.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://ofp.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://vip.pycfn.com

Java: resp.statusCode()
来源：http://zsg.sufxvd.cn

Go:   resp.StatusCode
来源：http://kbi.smart0.xyz

Ruby: resp.code.to_i
来源：http://jns.havefunace.top

C#:   (int)resp.StatusCode
来源：http://mwb.snrcjt.cn

[L08] 并发请求多个地址
来源：http://szs.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rma.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://zpo.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://upm.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hly.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ywj.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mzz.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uyt.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://veo.zdbjq.cn

================================================================================
来源：http://pzz.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://trm.hesvh.cn

================================================================================
来源：http://oja.andypj.xyz

[M01] 读取命令行参数
来源：http://rxn.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://vmc.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://iew.cucudq.cn

JS:   process.argv.slice(2)
来源：http://oyx.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://psg.yj202588.top

Java: args 数组（main 方法参数）
来源：http://cnr.havefunace.top

Go:   os.Args[1:]
来源：http://pgs.fzhhl.top

Ruby: ARGV
来源：http://ulk.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://jod.cdnleiting.top

[M02] 读取环境变量
来源：http://kgz.sweek.top

Py:   os.environ.get("HOME")
来源：http://cnz.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yes.tian-w.cn

JS:   process.env.HOME
来源：http://flv.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://xmz.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://bvs.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bse.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://oda.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://apu.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://hcg.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nkx.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://omp.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://yqv.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jzp.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kaw.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ftl.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://vgk.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://xqh.xinyue.icu

[M04] 获取当前工作目录
来源：http://qpw.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://uof.yj202588.top

PHP:  getcwd();
来源：http://deq.cashguo.top

JS:   process.cwd()
来源：http://bxw.nanxuanxn.top

TS:   process.cwd()
来源：http://qvu.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://isy.shangyingyoupin.top

Go:   os.Getwd()
来源：http://gtq.yj202588.top

Ruby: Dir.pwd
来源：http://kww.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://yhk.fanxiaobao.xyz

[M05] 设置退出码
来源：http://nhr.chenlongwang.top

Py:   sys.exit(1)
来源：http://lny.shuidangran.top

PHP:  exit(1);
来源：http://xfv.guowangkeji.top

JS:   process.exit(1)
来源：http://qdw.wangshuangyany.cn

TS:   process.exit(1)
来源：http://oub.feifeiyinyue.top

Java: System.exit(1)
来源：http://nst.yuxming.cn

Go:   os.Exit(1)
来源：http://sxi.yj202588.top

Ruby: exit 1
来源：http://jch.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qoz.vqdsnc.cn

[M06] 向标准错误输出
来源：http://scg.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://qmv.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ful.hnxiangtu.top

JS:   console.error("err")
来源：http://pxa.vqdsnc.cn

TS:   console.error("err")
来源：http://jid.9152youxi.cn

Java: System.err.println("err")
来源：http://pne.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yif.svipenyu.cn

Ruby: warn "err"
来源：http://qmu.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://nco.svipenyu.cn

[M07] 判断是否为主入口
来源：http://ftq.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://vwj.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yof.cucudq.cn

JS:   require.main === module
来源：http://cci.zdbjq.cn

TS:   require.main === module
来源：http://hni.cqqwz.cn

Java: public static void main(String[] args)
来源：http://onp.guannengcc.top

Go:   func main()
来源：http://lws.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bdb.yj202588.top

C#:   static void Main(string[] args)
来源：http://jbi.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://qia.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://omo.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://fvd.52xcode.cn

JS:   process.platform;  process.version
来源：http://xij.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://elz.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wtg.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gse.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jof.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nev.hongshengwenyu.top

================================================================================
来源：http://zss.shzxlz.cn

N. 数据结构与算法
来源：http://xea.daxiang520.top

================================================================================
来源：http://rbq.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://gyt.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hxi.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://csx.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eth.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jgm.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kuc.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://okh.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fcb.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ysd.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://vxx.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://uxa.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fqr.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://enb.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ogz.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://irh.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://lxe.feifeiyinyue.top

Ruby: arr.sort
来源：http://bvn.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wel.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://xmc.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uhb.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://hbx.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dgu.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvy.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xef.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vbd.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://flg.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://phn.nanxuanxn.top

[N04] 斐波那契数列
来源：http://bry.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vfl.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zfv.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vub.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnw.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ogf.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tsr.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sjv.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rbv.jinqigfzy.top

[N05] 最大公约数
来源：http://qdf.uphjek.com

Py:   math.gcd(a, b)
来源：http://omn.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kzf.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eom.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqf.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://foc.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yrf.smart0.xyz

Ruby: a.gcd(b)
来源：http://vpg.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tlk.yj20258888.top

[N06] 判断回文字符串
来源：http://rdi.ctjpmb.com

Py:   s == s[::-1]
来源：http://ujk.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://lix.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://hsu.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://zgn.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wqy.jianghu66.top

Go:   // 双指针从两端比较
来源：http://hrg.birdmap.top

Ruby: s == s.reverse
来源：http://wrp.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://udu.yj20258.top

[N07] 两数之和（返回下标）
来源：http://qrp.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yad.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pcg.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cyw.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://hde.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://smc.xinyue.icu

Go:   // 手写 map[int]int
来源：http://cxr.tianlin.xyz

Ruby: // 手写 Hash
来源：http://vgb.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://yol.zhijiandao.cn

[N08] 生成全排列
来源：http://npp.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://mhe.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://ths.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://svj.hywenlv.cn

TS:   // 手写回溯递归
来源：http://uxe.jinqigufen.top

Java: // 手写回溯递归
来源：http://xbi.xinyue.icu

Go:   // 手写回溯递归
来源：http://vud.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://icq.sxryk.cn

C#:   // 手写回溯递归
来源：http://fsq.vehdjk.com

[N09] 栈与队列
来源：http://hhz.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nwh.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://two.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mvk.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tep.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://med.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ili.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zvr.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ala.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://aeu.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ara.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://krm.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dqa.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dko.yonumen.top

Java: class Node { int v; Node next; }
来源：http://aas.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vbe.ppjwa.cn


<!-- 参考信息 -->