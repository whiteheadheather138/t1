代发 wailian999

TS:   JSON.parse(s)
来源：http://umd.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tmh.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://ibs.52xcode.cn

Ruby: JSON.parse(s)
来源：http://ntx.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://psx.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://kre.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ipt.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uaw.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ryb.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fot.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yww.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sxw.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://mlo.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aud.jianghu66.top

[K04] 读取 JSON 文件
来源：http://lef.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bqm.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ons.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xsy.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxe.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rwp.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://caw.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dla.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wsr.zhoulong.xyz

[K05] 深拷贝对象
来源：http://oep.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://xbc.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://loo.jyoumei.cn

JS:   structuredClone(obj)
来源：http://nxq.zhixingplan.top

TS:   structuredClone(obj)
来源：http://khy.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wzd.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zfw.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nbf.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ilo.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://poy.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bmr.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lrk.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lup.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrc.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pfx.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tay.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iir.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nsr.kuanghao11.cn

[K07] 进制转换
来源：http://hkt.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxn.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://puf.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uyn.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uni.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://otq.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sdf.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rdo.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jwt.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://kxz.cheryme.top

Py:   pickle.dumps(obj)
来源：http://afs.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://nvu.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://ddp.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://lci.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gdo.xylfe.cn

Go:   encoding/gob
来源：http://xbs.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://aiv.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eax.chenlongwang.top

================================================================================
来源：http://ejg.ybcxt.top

L. 网络请求
来源：http://ljf.316326.xyz

================================================================================
来源：http://ouz.ybcxt.top

[L01] 发送 GET 请求
来源：http://lkt.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://abk.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bxi.cashguo.top

JS:   await fetch(url)
来源：http://qzg.tanke756.top

TS:   await fetch(url)
来源：http://sxw.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uxt.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://ksw.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://wwk.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrj.fzhhl.top

[L02] 发送 POST JSON
来源：http://htk.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://gxr.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xya.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zls.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccx.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nag.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rjh.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmq.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gjp.andypj.xyz

[L03] 设置自定义请求头
来源：http://azh.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gcx.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jkm.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzr.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://glq.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hyh.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xub.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mfa.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gdh.daria6918.cn

[L04] 设置超时
来源：http://szr.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://fwt.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hea.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ifj.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tlz.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vzb.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jqb.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vau.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jpn.sysykeji.top

[L05] 上传文件（multipart）
来源：http://iaf.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gkf.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kij.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wka.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyk.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hod.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ptw.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zlt.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gjv.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://tbi.tianlin.xyz

Py:   resp.json()
来源：http://lfv.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://pjk.chenzaomai.com

JS:   await resp.json()
来源：http://hku.feifeiyinyue.top

TS:   await resp.json()
来源：http://tvb.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ohm.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lsg.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://ezb.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ujq.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://cmw.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qfq.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bik.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://mct.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://wgs.zhengqikj.top

Java: resp.statusCode()
来源：http://tox.cucudq.cn

Go:   resp.StatusCode
来源：http://ksp.ydzc1.top

Ruby: resp.code.to_i
来源：http://gia.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://qzh.yangfankeji.com

[L08] 并发请求多个地址
来源：http://sfu.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://idj.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://opc.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xlc.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ils.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kfb.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://izl.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vgh.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bmp.bjfxy.top

================================================================================
来源：http://fjv.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://zvw.zdqjudy.top

================================================================================
来源：http://dpj.tianlin.xyz

[M01] 读取命令行参数
来源：http://fjt.jyoumei.cn

Py:   sys.argv[1:]
来源：http://qnp.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://tfv.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://nto.hesvh.cn

TS:   process.argv.slice(2)
来源：http://xqa.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://anj.0kj1m.cn

Go:   os.Args[1:]
来源：http://ffx.chenzaomai.com

Ruby: ARGV
来源：http://ggo.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://rzi.yj20258.top

[M02] 读取环境变量
来源：http://eeh.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://ejy.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://foj.hywenlv.cn

JS:   process.env.HOME
来源：http://xdo.fktsv.cn

TS:   process.env.HOME
来源：http://ohx.nwbrower.top

Java: System.getenv("HOME")
来源：http://idg.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dtc.sweek.top

Ruby: ENV["HOME"]
来源：http://hke.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rdz.yfazqb.com

[M03] 执行外部命令
来源：http://tpd.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpc.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://znw.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ymu.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vdo.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jbr.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fvv.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://tbc.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://cec.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://wbm.smart0.xyz

Py:   os.getcwd()
来源：http://ete.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://ufq.iojbl.cn

JS:   process.cwd()
来源：http://rxq.cashguo.top

TS:   process.cwd()
来源：http://cdw.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://qqu.cheryme.top

Go:   os.Getwd()
来源：http://vgg.chenzaomai.com

Ruby: Dir.pwd
来源：http://opv.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dqe.xziqi.cn

[M05] 设置退出码
来源：http://qox.0kj1m.cn

Py:   sys.exit(1)
来源：http://hfj.hnxiangtu.top

PHP:  exit(1);
来源：http://gyd.shuidangran.top

JS:   process.exit(1)
来源：http://zfa.smart0.xyz

TS:   process.exit(1)
来源：http://mez.sysykeji.top

Java: System.exit(1)
来源：http://cko.havefunace.top

Go:   os.Exit(1)
来源：http://wqi.sjlbkw.cn

Ruby: exit 1
来源：http://xud.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sax.sjlbkw.cn

[M06] 向标准错误输出
来源：http://plj.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://znx.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iki.shzxlz.cn

JS:   console.error("err")
来源：http://drs.zhijiandao.cn

TS:   console.error("err")
来源：http://wbg.bjfxy.top

Java: System.err.println("err")
来源：http://spy.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://plw.fehbvm.com

Ruby: warn "err"
来源：http://nyh.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://ypy.yj202588.top

[M07] 判断是否为主入口
来源：http://rkc.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://lgp.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vjs.fktsv.cn

JS:   require.main === module
来源：http://bwt.yj20258888.top

TS:   require.main === module
来源：http://kxk.gzhubu.top

Java: public static void main(String[] args)
来源：http://orj.hnxiangtu.top

Go:   func main()
来源：http://mwm.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xrb.tian-w.cn

C#:   static void Main(string[] args)
来源：http://wob.pycfn.com

[M08] 获取系统与运行时信息
来源：http://twg.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://cpu.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://svg.sysykeji.top

JS:   process.platform;  process.version
来源：http://fva.chenlongwang.top

TS:   process.platform;  process.version
来源：http://qlv.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ykg.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bgb.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dfd.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lwa.ctjpmb.com

================================================================================
来源：http://ffq.zhiwuduotai.top

N. 数据结构与算法
来源：http://dlc.xylfe.cn

================================================================================
来源：http://ojq.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://lmd.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://pen.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://own.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msn.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsv.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://giv.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://nfw.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kfs.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://sbo.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://kty.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://jbd.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pjf.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bdq.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ffo.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://neh.guannengcc.top

Go:   slices.Sort(arr)
来源：http://qpy.hfpthk.cn

Ruby: arr.sort
来源：http://ini.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyd.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://tpu.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ppf.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://cys.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sfs.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yjf.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pgc.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wok.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mfs.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://yct.zhoulong.xyz

[N04] 斐波那契数列
来源：http://uqh.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zyw.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eek.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjw.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lyc.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bjk.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vuk.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hin.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://njt.wangshuangyany.cn

[N05] 最大公约数
来源：http://utc.sweek.top

Py:   math.gcd(a, b)
来源：http://dwq.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sfz.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ppw.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyg.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bmw.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sdf.yuxming.cn

Ruby: a.gcd(b)
来源：http://cso.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bxh.hcnkem.com

[N06] 判断回文字符串
来源：http://dmq.kuanghao11.cn

Py:   s == s[::-1]
来源：http://das.hnqzz.top

PHP:  $s === strrev($s);
来源：http://jcu.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://ice.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://odj.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ixs.daria6918.cn

Go:   // 双指针从两端比较
来源：http://blk.hnxiangtu.top

Ruby: s == s.reverse
来源：http://kov.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gmd.yongpay.top

[N07] 两数之和（返回下标）
来源：http://emn.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qxb.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dbq.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vds.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://qdh.yuanzhike.top

Java: // 手写 HashMap
来源：http://bod.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://trj.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://xga.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ruk.redwolf501.top

[N08] 生成全排列
来源：http://prm.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://fao.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://for.ehwqpu.com

JS:   // 手写回溯递归
来源：http://jsz.ydzc1.top

TS:   // 手写回溯递归
来源：http://xgp.daria6918.cn

Java: // 手写回溯递归
来源：http://fln.yangfankeji.com

Go:   // 手写回溯递归
来源：http://ekl.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://tyq.yuanzhike.top

C#:   // 手写回溯递归
来源：http://iqw.meibo888.top

[N09] 栈与队列
来源：http://zno.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wck.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yoe.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oaa.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vjn.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gnw.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://osk.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gqy.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wmd.tian-w.cn

[N10] 链表节点定义
来源：http://kbv.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fhp.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oht.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dtx.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://woi.pycfn.com

Java: class Node { int v; Node next; }
来源：http://dzj.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://ddq.zhixingplan.top


<!-- 参考信息 -->