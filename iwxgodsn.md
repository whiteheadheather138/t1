代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://izi.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ady.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://avx.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://bkl.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gff.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dds.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlu.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://otv.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fkg.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owo.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://euy.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vwk.vqdsnc.cn

================================================================================
来源：http://gxh.hcnkem.com

K. JSON 与序列化
来源：http://fso.shanyushiyangtech.top

================================================================================
来源：http://ids.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://yav.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heo.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xzu.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://ezv.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://epi.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tfx.xylfe.cn

Go:   json.Marshal(obj)
来源：http://ikn.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://sgs.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://itq.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://cbj.yvedp.cn

Py:   json.loads(s)
来源：http://ozu.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcr.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://qel.havefunace.top

TS:   JSON.parse(s)
来源：http://bsi.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lcp.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://xtr.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://wdp.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hlq.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://xcw.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://njf.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nct.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gxd.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bcs.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qip.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yye.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hww.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://osw.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://yoa.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://myz.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lra.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dnl.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yxz.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bdu.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://drs.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eqq.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://guj.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://lkg.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://kxu.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://yrg.zdbjq.cn

JS:   structuredClone(obj)
来源：http://zcm.iojbl.cn

TS:   structuredClone(obj)
来源：http://udw.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rmq.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nqm.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uoa.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bho.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://rnt.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://syk.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ydq.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mcm.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ohn.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tgh.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gat.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lvf.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iby.meibo888.top

[K07] 进制转换
来源：http://xfw.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yqz.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rxh.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uml.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gyw.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xyu.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kjp.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rpe.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zku.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://liv.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://urm.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://yvt.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yyq.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://zha.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fpx.ppjwa.cn

Go:   encoding/gob
来源：http://tjm.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://sxk.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://krh.vqdsnc.cn

================================================================================
来源：http://gov.bbcook.cn

L. 网络请求
来源：http://cbl.hnxiangtu.top

================================================================================
来源：http://cxg.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://ulz.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pfr.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ypi.havefunace.top

JS:   await fetch(url)
来源：http://bkv.hfpthk.cn

TS:   await fetch(url)
来源：http://afz.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gmi.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://ymy.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qcf.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pkv.yuanzhike.top

[L02] 发送 POST JSON
来源：http://pkt.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://aah.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iyt.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dch.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://loe.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kbv.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mzh.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvz.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qkn.nanxinkj.top

[L03] 设置自定义请求头
来源：http://cgi.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pst.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yxv.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rnr.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehg.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qmz.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lwh.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fwb.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vcr.smart0.xyz

[L04] 设置超时
来源：http://xie.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://ywi.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xqg.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wil.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ljn.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rra.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tjf.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gle.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pbk.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://rxh.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ham.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yxn.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wue.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rvd.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sps.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mrp.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://spb.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nyy.iojbl.cn

[L06] 解析响应为 JSON
来源：http://efh.ydzc1.top

Py:   resp.json()
来源：http://orz.ydzc1.top

PHP:  json_decode($body, true);
来源：http://jap.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://cie.feifeiyinyue.top

TS:   await resp.json()
来源：http://jqu.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iiq.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://znt.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://fui.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iko.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://rdt.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xxt.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nhq.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://nmm.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://cce.havefunace.top

Java: resp.statusCode()
来源：http://lwu.jqgufenzy.top

Go:   resp.StatusCode
来源：http://jkq.zhixingplan.top

Ruby: resp.code.to_i
来源：http://wmq.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://odr.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://tdv.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rli.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://lfq.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://num.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://otw.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nwo.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vrc.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wzu.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ido.sysykeji.top

================================================================================
来源：http://deb.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://eyt.zhiwuduotai.top

================================================================================
来源：http://lly.yj20258888.top

[M01] 读取命令行参数
来源：http://hkk.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://haf.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://nwc.yj20258888.top

JS:   process.argv.slice(2)
来源：http://szf.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://pcs.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://tee.xziqi.cn

Go:   os.Args[1:]
来源：http://sab.chenlongwang.top

Ruby: ARGV
来源：http://oyv.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://vqh.yanxiufei.cn

[M02] 读取环境变量
来源：http://lkb.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://pik.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qau.haohaochexian.top

JS:   process.env.HOME
来源：http://mpq.shuidangran.top

TS:   process.env.HOME
来源：http://ruc.yongpay.top

Java: System.getenv("HOME")
来源：http://voz.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://myw.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://yii.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tgy.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://zaw.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ade.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dxy.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gnv.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kmo.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nrp.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tmt.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://loi.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://sfp.tarul.cn

[M04] 获取当前工作目录
来源：http://brf.uphjek.com

Py:   os.getcwd()
来源：http://sdn.hywenlv.cn

PHP:  getcwd();
来源：http://oyp.jianghu66.top

JS:   process.cwd()
来源：http://lpl.yvedp.cn

TS:   process.cwd()
来源：http://pra.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://pic.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://ofy.daxiang520.top

Ruby: Dir.pwd
来源：http://ldp.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://pzm.52xcode.cn

[M05] 设置退出码
来源：http://dpr.tanke756.top

Py:   sys.exit(1)
来源：http://vai.mhx1999.top

PHP:  exit(1);
来源：http://rxo.aizwys.cn

JS:   process.exit(1)
来源：http://mhb.aizwys.cn

TS:   process.exit(1)
来源：http://fkt.cashguo.top

Java: System.exit(1)
来源：http://qfu.sweek.top

Go:   os.Exit(1)
来源：http://edc.jinqigufen.top

Ruby: exit 1
来源：http://jdw.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hta.chenzaomai.com

[M06] 向标准错误输出
来源：http://enb.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://ktl.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mpz.chenlongwang.top

JS:   console.error("err")
来源：http://tom.yangfankeji.com

TS:   console.error("err")
来源：http://vdl.xylfe.cn

Java: System.err.println("err")
来源：http://izw.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ykc.jqgufenzy.top

Ruby: warn "err"
来源：http://fmi.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://xfs.bbcook.cn

[M07] 判断是否为主入口
来源：http://pmz.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://lmf.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wmu.zhixingplan.top

JS:   require.main === module
来源：http://nbw.cdnleiting.top

TS:   require.main === module
来源：http://qky.ctjpmb.com

Java: public static void main(String[] args)
来源：http://roq.ydzc1.top

Go:   func main()
来源：http://iau.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hlm.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://iow.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://ydw.xinyue.icu

Py:   platform.system();  platform.python_version()
来源：http://oem.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://xpc.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://olo.yangfankeji.com

TS:   process.platform;  process.version
来源：http://jqr.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mmp.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://clc.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yfd.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://swh.aizwys.cn

================================================================================
来源：http://lsf.jqgfzy.top

N. 数据结构与算法
来源：http://cak.yangfankeji.com

================================================================================
来源：http://kyz.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://oni.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://usr.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uyv.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idl.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qiv.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dwy.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://tgl.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vyp.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://kre.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://qmr.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://pdw.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vju.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rvm.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gjk.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbv.meibo888.top

Go:   slices.Sort(arr)
来源：http://mpw.chenzaomai.com

Ruby: arr.sort
来源：http://cye.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bjk.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://udz.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iqm.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://ivp.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ncy.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ucb.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gwo.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wyg.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cis.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://xoz.jiagoushi.top

[N04] 斐波那契数列
来源：http://ydc.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fal.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://amz.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vri.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aan.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xln.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbb.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xcq.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ekk.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://kck.fzhhl.top

Py:   math.gcd(a, b)
来源：http://xaa.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://igm.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcg.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxc.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sbu.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://evy.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://oes.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xbp.sxryk.cn

[N06] 判断回文字符串
来源：http://taf.yanxiufei.cn

Py:   s == s[::-1]
来源：http://jyx.guannengcc.top

PHP:  $s === strrev($s);
来源：http://yhf.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://jcu.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://nyc.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nka.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://zbu.nwbrower.top

Ruby: s == s.reverse
来源：http://aeb.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lmy.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://mqe.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nce.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nqt.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tiu.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://suj.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://bqn.fzhhl.top


<!-- 参考信息 -->