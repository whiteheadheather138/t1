代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://liq.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://axi.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ols.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ezd.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ehq.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nxv.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lad.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uut.vqdsnc.cn

================================================================================
来源：http://ktq.aizwys.cn

K. JSON 与序列化
来源：http://gvd.nwbrower.top

================================================================================
来源：http://lxb.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://zcb.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zpj.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zcq.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://imq.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://onv.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bcr.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://obs.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aet.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dbu.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://puk.zhoulong.xyz

Py:   json.loads(s)
来源：http://nlm.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vou.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://kpn.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://dms.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://meq.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://zsp.c1oappe.top

Ruby: JSON.parse(s)
来源：http://plx.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyu.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://seh.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qrk.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://web.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xdy.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bfr.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gev.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwx.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://egy.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sai.xylfe.cn

[K04] 读取 JSON 文件
来源：http://ojt.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gyq.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xpl.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqw.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bdr.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bkb.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uju.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://het.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ffn.haohaochexian.top

[K05] 深拷贝对象
来源：http://vog.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://gnl.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://obl.jianghu66.top

JS:   structuredClone(obj)
来源：http://qdo.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://gnq.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mwc.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tnf.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsx.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xzc.c1oappe.top

[K06] 解析 URL 查询串
来源：http://dbe.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xeo.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jrm.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ekb.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bcp.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxd.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://sqb.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bhp.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hqi.wangshuangyany.cn

[K07] 进制转换
来源：http://qyr.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ybu.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqk.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qhl.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ytn.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://spk.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fpq.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://trl.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzn.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://lef.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://fme.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xwi.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://cad.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://kjf.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qvc.meibo888.top

Go:   encoding/gob
来源：http://ryw.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://mgc.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ixc.gotoacloud.top

================================================================================
来源：http://xuf.feifeiyinyue.top

L. 网络请求
来源：http://jqf.vqdsnc.cn

================================================================================
来源：http://hfd.c1oappe.top

[L01] 发送 GET 请求
来源：http://tyb.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zlg.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bpp.iojbl.cn

JS:   await fetch(url)
来源：http://tjn.zdqjudy.top

TS:   await fetch(url)
来源：http://pqm.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yzv.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://lul.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://htq.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ujm.jiagoushi.top

[L02] 发送 POST JSON
来源：http://gpc.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://ovm.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zev.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tdf.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gep.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugw.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dcb.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oaj.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vnr.cqqwz.cn

[L03] 设置自定义请求头
来源：http://xjb.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://etd.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bvq.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emi.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nxt.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wnl.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mju.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cfw.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fmi.svipenyu.cn

[L04] 设置超时
来源：http://wlt.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://sck.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jic.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvf.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xve.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lnp.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rrb.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fkt.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pld.andypj.xyz

[L05] 上传文件（multipart）
来源：http://wiq.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ldl.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqb.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://erv.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kbi.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dov.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ybh.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fmg.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://isz.yfazqb.com

[L06] 解析响应为 JSON
来源：http://psb.nanxuanxn.top

Py:   resp.json()
来源：http://pks.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://dvm.hnxiangtu.top

JS:   await resp.json()
来源：http://xet.yuxming.cn

TS:   await resp.json()
来源：http://omo.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fth.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bty.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://dcc.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hpc.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://agb.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lkm.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://akz.sweek.top

JS:   resp.ok;  resp.status
来源：http://bcs.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://pfk.chenzaomai.com

Java: resp.statusCode()
来源：http://wum.fzhhl.top

Go:   resp.StatusCode
来源：http://dhp.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://mbf.tarul.cn

C#:   (int)resp.StatusCode
来源：http://fty.hammf.cn

[L08] 并发请求多个地址
来源：http://pbf.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cje.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://kmc.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhj.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnr.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hss.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ryc.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pto.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ooa.birdmap.top

================================================================================
来源：http://eqq.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://hhn.bbcook.cn

================================================================================
来源：http://itj.zhijiandao.cn

[M01] 读取命令行参数
来源：http://zkm.52xcode.cn

Py:   sys.argv[1:]
来源：http://ggv.mhx1999.top

PHP:  $argv;  $argc;
来源：http://quj.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://jbi.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://pmu.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://ide.yueranfly.top

Go:   os.Args[1:]
来源：http://nzd.tarul.cn

Ruby: ARGV
来源：http://giw.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://kbv.fengsongda.top

[M02] 读取环境变量
来源：http://dgy.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://zor.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gnl.cucudq.cn

JS:   process.env.HOME
来源：http://pyw.cheryme.top

TS:   process.env.HOME
来源：http://gjr.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://xgd.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jyx.tanke756.top

Ruby: ENV["HOME"]
来源：http://sfw.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://raf.tarul.cn

[M03] 执行外部命令
来源：http://imh.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wxf.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dlv.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ypo.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ull.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zoa.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eam.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ifp.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://ekh.daxiang520.top

[M04] 获取当前工作目录
来源：http://iwc.cashguo.top

Py:   os.getcwd()
来源：http://qty.chenjidiqi.icu

PHP:  getcwd();
来源：http://qam.zhiwuduotai.top

JS:   process.cwd()
来源：http://tmt.cdnleiting.top

TS:   process.cwd()
来源：http://ofv.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://cir.quarkkingdee.top

Go:   os.Getwd()
来源：http://bre.yj202588.top

Ruby: Dir.pwd
来源：http://ioj.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://oyz.c1oappe.top

[M05] 设置退出码
来源：http://onf.andypj.xyz

Py:   sys.exit(1)
来源：http://bsm.zhengqikj.top

PHP:  exit(1);
来源：http://wnb.hnxiangtu.top

JS:   process.exit(1)
来源：http://swo.fktsv.cn

TS:   process.exit(1)
来源：http://pij.zycfv.cn

Java: System.exit(1)
来源：http://kyd.haohaochexian.top

Go:   os.Exit(1)
来源：http://rqg.xuetiantiany.cn

Ruby: exit 1
来源：http://ujt.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nay.yueranfly.top

[M06] 向标准错误输出
来源：http://svx.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://ldr.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zvx.tanke756.top

JS:   console.error("err")
来源：http://nth.xinyue.icu

TS:   console.error("err")
来源：http://vct.hnqzz.top

Java: System.err.println("err")
来源：http://fmy.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqc.cdnleiting.top

Ruby: warn "err"
来源：http://ngg.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://bop.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://smb.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://abx.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bwx.zdbjq.cn

JS:   require.main === module
来源：http://uhw.jqgufenzy.top

TS:   require.main === module
来源：http://pcv.yj20258.top

Java: public static void main(String[] args)
来源：http://jbo.snrcjt.cn

Go:   func main()
来源：http://zgb.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cth.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://bfl.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://jga.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://aec.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://daq.chenzaomai.com

JS:   process.platform;  process.version
来源：http://vwg.shuidangran.top

TS:   process.platform;  process.version
来源：http://dwl.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zev.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mzp.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ned.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://try.redwolf501.top

================================================================================
来源：http://mhb.hcnkem.com

N. 数据结构与算法
来源：http://any.zhaomingkeji.xyz

================================================================================
来源：http://tlo.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://wym.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nuu.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ufn.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hha.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nom.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://plv.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://dbc.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ywd.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://dqz.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://yyy.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://lcb.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gqm.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qns.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sii.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hkl.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://juj.zhongyouzk.top

Ruby: arr.sort
来源：http://cgj.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gta.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://sfb.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mey.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://nig.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zoc.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://koc.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yhh.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tlj.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dxr.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://ayw.andypj.xyz

[N04] 斐波那契数列
来源：http://yjc.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ziu.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://riq.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://erh.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lek.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fjk.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fip.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jye.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://phr.cucudq.cn

[N05] 最大公约数
来源：http://rmk.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://awg.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jmy.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iuu.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vgi.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwu.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zne.gotoacloud.top

Ruby: a.gcd(b)
来源：http://jaw.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ywm.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://ouu.hesvh.cn

Py:   s == s[::-1]
来源：http://dfl.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://qrj.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://qyi.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://nhl.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lcs.hesvh.cn

Go:   // 双指针从两端比较
来源：http://bfp.zhongyouzk.top

Ruby: s == s.reverse
来源：http://yjh.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yno.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://nnn.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://czy.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jiu.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yzg.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://yhd.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://fjp.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://lml.birdmap.top

Ruby: // 手写 Hash
来源：http://qqa.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://cdr.gogol.net.cn

[N08] 生成全排列
来源：http://lhm.guannengcc.top


<!-- 参考信息 -->