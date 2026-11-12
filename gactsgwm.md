代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xke.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gra.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnn.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bah.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ojm.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pak.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tbv.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://tip.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tpd.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mlx.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nhb.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bgx.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ewn.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bue.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfx.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbx.fehbvm.com

================================================================================
来源：http://wbu.ydzc1.top

K. JSON 与序列化
来源：http://zzq.jiagoushi.top

================================================================================
来源：http://gbc.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://nab.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mow.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ygn.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://bhn.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://iwp.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xeu.yj202588.top

Go:   json.Marshal(obj)
来源：http://fpg.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wuq.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tcl.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://uda.xuanzx.com

Py:   json.loads(s)
来源：http://njw.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mlw.epnwcf.com

JS:   JSON.parse(s)
来源：http://qga.jiagoushi.top

TS:   JSON.parse(s)
来源：http://nzf.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jcr.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://lcg.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://mvz.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fmf.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://suy.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qiu.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://seu.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kgu.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yzz.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://csi.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qky.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://ilk.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eac.yuxming.cn

[K04] 读取 JSON 文件
来源：http://udv.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qbv.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kcf.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://flz.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eof.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://obz.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://phk.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sko.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xxv.fktsv.cn

[K05] 深拷贝对象
来源：http://lzl.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://dki.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://cqp.svipenyu.cn

JS:   structuredClone(obj)
来源：http://vxr.cqqwz.cn

TS:   structuredClone(obj)
来源：http://aat.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nsj.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://era.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vja.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://qhz.yj20258.top

[K06] 解析 URL 查询串
来源：http://fur.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xdd.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ddj.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eec.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hpn.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bnq.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rxj.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wok.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cjb.havefunace.top

[K07] 进制转换
来源：http://ulj.zdqjudy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vpd.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dih.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ipp.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bwi.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nxv.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jym.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://exm.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bue.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://boa.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://gix.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lpj.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://tqy.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://eub.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ouk.haohaochexian.top

Go:   encoding/gob
来源：http://kqs.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://zfw.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://djb.zdqjudy.top

================================================================================
来源：http://ake.vehdjk.com

L. 网络请求
来源：http://vtx.shanyushiyangkeji.top

================================================================================
来源：http://khg.yueranfly.top

[L01] 发送 GET 请求
来源：http://hdq.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://arr.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rdh.pycfn.com

JS:   await fetch(url)
来源：http://ghy.zhijiandao.cn

TS:   await fetch(url)
来源：http://azu.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://voh.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://ero.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fvs.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://krh.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://umm.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://lxa.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nwd.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ube.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bed.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eui.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yoc.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://keg.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dix.redwolf501.top

[L03] 设置自定义请求头
来源：http://eyw.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://apr.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://knh.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://maa.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgq.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gft.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xqu.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qsd.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yge.zhiwuduotai.top

[L04] 设置超时
来源：http://lmv.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://gsf.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lru.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nox.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwn.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zdj.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://knr.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ata.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hir.yj202588.top

[L05] 上传文件（multipart）
来源：http://soq.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vva.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wxy.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eot.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://czs.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ioj.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hbo.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kaa.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oba.sweek.top

[L06] 解析响应为 JSON
来源：http://yxm.ehwqpu.com

Py:   resp.json()
来源：http://oni.zycfv.cn

PHP:  json_decode($body, true);
来源：http://kxe.xuanzx.com

JS:   await resp.json()
来源：http://mou.cheryme.top

TS:   await resp.json()
来源：http://wni.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pqi.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://arr.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://cky.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ibe.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://gtx.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://moc.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mio.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://hmk.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://bzc.jqgfzy.top

Java: resp.statusCode()
来源：http://gjq.0kj1m.cn

Go:   resp.StatusCode
来源：http://rkj.shzxlz.cn

Ruby: resp.code.to_i
来源：http://pux.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://igq.jqgfzy.top

[L08] 并发请求多个地址
来源：http://nap.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://evb.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://gji.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swl.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://beh.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dga.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aoi.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qyf.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mlz.c1oappe.top

================================================================================
来源：http://pxe.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://wxf.daria6918.cn

================================================================================
来源：http://iop.ivvv.top

[M01] 读取命令行参数
来源：http://hpz.birdmap.top

Py:   sys.argv[1:]
来源：http://rsq.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://aqq.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://ikn.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://pks.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://rdm.cheryme.top

Go:   os.Args[1:]
来源：http://yds.yueranfly.top

Ruby: ARGV
来源：http://nwr.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://wwd.jiagoushi.top

[M02] 读取环境变量
来源：http://via.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://oyc.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fxg.52xcode.cn

JS:   process.env.HOME
来源：http://ggc.wangshuangyany.cn

TS:   process.env.HOME
来源：http://xsl.smart0.xyz

Java: System.getenv("HOME")
来源：http://cak.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://urv.fehbvm.com

Ruby: ENV["HOME"]
来源：http://kxd.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xvl.uphjek.com

[M03] 执行外部命令
来源：http://bgi.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lrn.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fbg.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uot.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lvp.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nak.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aar.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://ika.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://llh.iojbl.cn

[M04] 获取当前工作目录
来源：http://fhx.yfazqb.com

Py:   os.getcwd()
来源：http://atm.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://biw.nwbrower.top

JS:   process.cwd()
来源：http://ixd.smart0.xyz

TS:   process.cwd()
来源：http://czf.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://jxd.zhiwuduotai.top

Go:   os.Getwd()
来源：http://hcw.fzhhl.top

Ruby: Dir.pwd
来源：http://prp.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mot.daxiang520.top

[M05] 设置退出码
来源：http://azd.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://jfa.nanxinkj.top

PHP:  exit(1);
来源：http://vqa.fzhhl.top

JS:   process.exit(1)
来源：http://ujf.gaohongyu789.top

TS:   process.exit(1)
来源：http://quh.xinyue.icu

Java: System.exit(1)
来源：http://huj.yonumen.top

Go:   os.Exit(1)
来源：http://hvh.zhiwuduotai.top

Ruby: exit 1
来源：http://frv.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wql.havefunace.top

[M06] 向标准错误输出
来源：http://lld.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://zsi.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qxl.guowangkeji.top

JS:   console.error("err")
来源：http://ccr.hfpthk.cn

TS:   console.error("err")
来源：http://mwy.jinqigufen.top

Java: System.err.println("err")
来源：http://irl.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://byk.yfazqb.com

Ruby: warn "err"
来源：http://mmf.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://hor.jiagoushi.top

[M07] 判断是否为主入口
来源：http://mqs.birdmap.top

Py:   if __name__ == "__main__":
来源：http://qjz.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tgx.guowangkeji.top

JS:   require.main === module
来源：http://hww.yj202588.top

TS:   require.main === module
来源：http://sqo.nwbrower.top

Java: public static void main(String[] args)
来源：http://opp.shuidangran.top

Go:   func main()
来源：http://vzz.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://avo.yj20258.top

C#:   static void Main(string[] args)
来源：http://yyi.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://dag.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://qag.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://qvq.pycfn.com

JS:   process.platform;  process.version
来源：http://het.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://fqm.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://adh.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jni.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://swa.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jan.jinqigfzy.top

================================================================================
来源：http://acc.mhx1999.top

N. 数据结构与算法
来源：http://nzl.haohaochexian.top

================================================================================
来源：http://mbj.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://ovy.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nae.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nsb.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://guu.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdv.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://omg.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://zwp.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nab.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://esi.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://eti.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://heg.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yas.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gur.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eic.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iil.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://xnr.gogol.net.cn

Ruby: arr.sort
来源：http://knd.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://srk.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://ovo.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://arv.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://nxu.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ggu.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tqa.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fix.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sri.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hmv.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://hfo.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://dpv.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hwu.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uou.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dkm.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgs.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dud.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://odq.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dyr.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dbn.yvedp.cn

[N05] 最大公约数
来源：http://gzt.sxryk.cn

Py:   math.gcd(a, b)
来源：http://sff.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://skv.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oai.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xlo.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tsx.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uoz.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://mtk.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uvy.jiagoushi.top

[N06] 判断回文字符串
来源：http://xxk.hcnkem.com

Py:   s == s[::-1]
来源：http://yil.jianghu66.top

PHP:  $s === strrev($s);
来源：http://ucy.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://gfw.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://zqu.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ime.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://fxb.xinyue.icu

Ruby: s == s.reverse
来源：http://xzg.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vnq.yongpay.top

[N07] 两数之和（返回下标）
来源：http://fvs.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oyz.fzhhl.top


<!-- 参考信息 -->