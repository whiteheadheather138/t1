代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://unx.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://uhz.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://arz.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oub.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://emo.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://obd.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdf.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ggc.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://isw.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://idw.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://lmy.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afc.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://exv.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rst.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gea.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kma.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oos.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tdk.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mnx.daxiang520.top

[K05] 深拷贝对象
来源：http://xif.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://kub.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://xnn.316326.xyz

JS:   structuredClone(obj)
来源：http://owv.zdbjq.cn

TS:   structuredClone(obj)
来源：http://lel.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bog.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nfl.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cft.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://daw.iojbl.cn

[K06] 解析 URL 查询串
来源：http://xqi.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wou.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qhn.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mah.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vzn.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpm.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fhw.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvw.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://akx.birdmap.top

[K07] 进制转换
来源：http://ybf.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vzm.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://obd.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lxg.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ent.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hrd.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pqm.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://psv.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sjk.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://kyu.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://dkf.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qjz.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://nbc.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://lwx.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mik.hywenlv.cn

Go:   encoding/gob
来源：http://nqf.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://oyz.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://llm.yfazqb.com

================================================================================
来源：http://mer.52xcode.cn

L. 网络请求
来源：http://mqr.kuanghao11.cn

================================================================================
来源：http://pox.tanke756.top

[L01] 发送 GET 请求
来源：http://iih.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djg.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rhg.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://bcb.zdqjudy.top

TS:   await fetch(url)
来源：http://pyn.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lgq.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://daf.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lkn.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lwh.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://ron.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://sfn.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjl.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttw.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zux.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mmx.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oca.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rtb.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lfu.hnqzz.top

[L03] 设置自定义请求头
来源：http://dzp.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wqv.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dec.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwp.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://drj.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hkw.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zar.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eac.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qgq.0kj1m.cn

[L04] 设置超时
来源：http://uci.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://usv.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ais.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pna.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dow.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dvl.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sio.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ata.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ysc.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://vfx.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rmd.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://myc.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnd.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ahz.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://spj.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdq.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lgj.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://meb.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://iwo.zhengqikj.top

Py:   resp.json()
来源：http://oqt.xylfe.cn

PHP:  json_decode($body, true);
来源：http://jbl.guowangkeji.top

JS:   await resp.json()
来源：http://bej.sweek.top

TS:   await resp.json()
来源：http://khh.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sos.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vxm.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://wdz.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mcc.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://puf.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://afy.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hdd.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://ysz.yj20258.top

TS:   resp.ok;  resp.status
来源：http://gpo.tanke756.top

Java: resp.statusCode()
来源：http://vtc.fehbvm.com

Go:   resp.StatusCode
来源：http://eoe.ehwqpu.com

Ruby: resp.code.to_i
来源：http://ica.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://bwb.tanke756.top

[L08] 并发请求多个地址
来源：http://sdw.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vcf.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://zal.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uav.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://amw.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fcg.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qag.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tft.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xuf.hongshengwenyu.top

================================================================================
来源：http://wgw.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://cge.zdqjudy.top

================================================================================
来源：http://web.bbcook.cn

[M01] 读取命令行参数
来源：http://xom.yonumen.top

Py:   sys.argv[1:]
来源：http://jab.ydzc1.top

PHP:  $argv;  $argc;
来源：http://tjm.ybcxt.top

JS:   process.argv.slice(2)
来源：http://sdm.ivvv.top

TS:   process.argv.slice(2)
来源：http://bfl.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://ily.nwbrower.top

Go:   os.Args[1:]
来源：http://yzd.shzxlz.cn

Ruby: ARGV
来源：http://tjv.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://ozk.cheryme.top

[M02] 读取环境变量
来源：http://bzg.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://xrj.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fdh.yj202588.top

JS:   process.env.HOME
来源：http://gdk.smart0.xyz

TS:   process.env.HOME
来源：http://wkf.yangfankeji.com

Java: System.getenv("HOME")
来源：http://cum.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ncq.ydzc1.top

Ruby: ENV["HOME"]
来源：http://mmp.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zlo.uphjek.com

[M03] 执行外部命令
来源：http://kiz.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zdl.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wqv.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tnj.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://krw.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ssy.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dvm.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://bdy.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://shk.dianchejie.cn

[M04] 获取当前工作目录
来源：http://rjf.andypj.xyz

Py:   os.getcwd()
来源：http://osz.c1oappe.top

PHP:  getcwd();
来源：http://acd.fehbvm.com

JS:   process.cwd()
来源：http://uby.kuanghao11.cn

TS:   process.cwd()
来源：http://jbd.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://mui.chenzaomai.com

Go:   os.Getwd()
来源：http://oeq.chenzaomai.com

Ruby: Dir.pwd
来源：http://yut.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://ocg.cdnleiting.top

[M05] 设置退出码
来源：http://kzb.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://sjs.iojbl.cn

PHP:  exit(1);
来源：http://bpr.tarul.cn

JS:   process.exit(1)
来源：http://ycc.tarul.cn

TS:   process.exit(1)
来源：http://vwa.ivvv.top

Java: System.exit(1)
来源：http://her.guowangkeji.top

Go:   os.Exit(1)
来源：http://lxa.yj20258888.top

Ruby: exit 1
来源：http://qfj.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://agu.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://ygf.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://irz.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sfn.tian-w.cn

JS:   console.error("err")
来源：http://ywu.hesvh.cn

TS:   console.error("err")
来源：http://bni.zhijiandao.cn

Java: System.err.println("err")
来源：http://ycz.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nox.jqgufenzy.top

Ruby: warn "err"
来源：http://qmo.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://dxs.yj20258.top

[M07] 判断是否为主入口
来源：http://ymw.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://gjv.ppjwa.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://clb.uphjek.com

JS:   require.main === module
来源：http://ffn.gogol.net.cn

TS:   require.main === module
来源：http://ztu.nanxinkj.top

Java: public static void main(String[] args)
来源：http://ksk.shanyushiyangtech.top

Go:   func main()
来源：http://gwl.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gnx.yfazqb.com

C#:   static void Main(string[] args)
来源：http://alm.sxryk.cn

[M08] 获取系统与运行时信息
来源：http://nmd.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://cbb.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://bay.guowangkeji.top

JS:   process.platform;  process.version
来源：http://nzj.smart0.xyz

TS:   process.platform;  process.version
来源：http://icb.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uap.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://azh.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fse.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://sal.daria6918.cn

================================================================================
来源：http://ywa.aibaodan.cn

N. 数据结构与算法
来源：http://yog.sjlbkw.cn

================================================================================
来源：http://khz.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://wcc.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://wua.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pzc.pycfn.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysx.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvi.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nxq.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://vtx.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rpc.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://aru.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://bvj.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://dtt.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqc.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://edo.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fhz.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://szy.316326.xyz

Go:   slices.Sort(arr)
来源：http://gev.guannengcc.top

Ruby: arr.sort
来源：http://ctn.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cer.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://acy.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ddw.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://lun.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dtg.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbl.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ujd.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rqu.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wyg.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://ozy.kuanghao11.cn

[N04] 斐波那契数列
来源：http://jfy.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lyz.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zjz.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ayj.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mxs.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qfb.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://twu.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mvh.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ync.chenjidiqi.icu

[N05] 最大公约数
来源：http://aqv.fktsv.cn

Py:   math.gcd(a, b)
来源：http://tns.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gkh.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cqe.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpm.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nvh.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xhx.mhx1999.top

Ruby: a.gcd(b)
来源：http://sig.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ysw.zycfv.cn

[N06] 判断回文字符串
来源：http://wng.chenlongwang.top

Py:   s == s[::-1]
来源：http://sxp.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://twk.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://dab.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://rqu.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://joa.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://qlk.wangdashe.top

Ruby: s == s.reverse
来源：http://unc.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ptf.hammf.cn

[N07] 两数之和（返回下标）
来源：http://uha.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jhv.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://akg.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wzl.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://fpa.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://zvo.havefunace.top

Go:   // 手写 map[int]int
来源：http://log.sufxvd.cn

Ruby: // 手写 Hash
来源：http://hew.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://oye.zycfv.cn

[N08] 生成全排列
来源：http://enb.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://exh.iojbl.cn

PHP:  // 手写递归交换
来源：http://jyn.smart0.xyz

JS:   // 手写回溯递归
来源：http://umj.sysykeji.top

TS:   // 手写回溯递归
来源：http://guu.pycfn.com

Java: // 手写回溯递归
来源：http://zlc.tarul.cn

Go:   // 手写回溯递归
来源：http://gro.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://uwr.xylfe.cn

C#:   // 手写回溯递归
来源：http://vxh.daxiang520.top

[N09] 栈与队列
来源：http://vhj.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qog.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tpb.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sux.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://met.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zpi.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lhc.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pih.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ncs.chenlongwang.top

[N10] 链表节点定义
来源：http://hhi.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ufb.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xwg.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrf.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tyr.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://ocu.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dph.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://amx.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jlc.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://gvm.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://goo.sweek.top


<!-- 参考信息 -->