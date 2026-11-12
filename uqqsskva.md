代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wql.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ztv.shanyushiyangkeji.top

[J09] 时区处理
来源：http://nsh.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pun.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dsh.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ijv.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nab.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aog.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xht.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cvd.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://imy.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://wbb.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ncx.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ycc.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cex.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jgd.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zvl.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahq.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xxu.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qqo.yj20258.top

================================================================================
来源：http://gct.daria6918.cn

K. JSON 与序列化
来源：http://mdp.vehdjk.com

================================================================================
来源：http://zch.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://mix.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixq.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjp.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://fnj.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://fva.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fod.bbcook.cn

Go:   json.Marshal(obj)
来源：http://dii.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://ykz.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://voa.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://lvs.mhx1999.top

Py:   json.loads(s)
来源：http://jtq.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nrq.aibaodan.cn

JS:   JSON.parse(s)
来源：http://rjj.vehdjk.com

TS:   JSON.parse(s)
来源：http://hpx.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://btf.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://wwp.bbcook.cn

Ruby: JSON.parse(s)
来源：http://tmu.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nha.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://zes.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xte.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwg.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mlc.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://drn.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nex.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://som.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://lca.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fpq.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://vlx.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kgs.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bwy.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mze.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbs.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lus.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://csc.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ltf.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://flc.mhx1999.top

[K05] 深拷贝对象
来源：http://nzt.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://mku.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://epv.andypj.xyz

JS:   structuredClone(obj)
来源：http://zpu.ybcxt.top

TS:   structuredClone(obj)
来源：http://ozx.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kdp.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ucq.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ytp.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wwk.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://ero.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pdn.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qxq.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hru.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wbw.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fhb.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wif.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://afx.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rhc.cdnleiting.top

[K07] 进制转换
来源：http://cmy.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tuy.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dhg.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cnu.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tdq.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://efj.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uem.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zaa.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uxa.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://yym.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://wxi.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ier.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://aud.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://tpv.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mpx.sjlbkw.cn

Go:   encoding/gob
来源：http://axw.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://kfd.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sdk.fktsv.cn

================================================================================
来源：http://wuq.hnqzz.top

L. 网络请求
来源：http://mjl.cdnleiting.top

================================================================================
来源：http://zni.hnqzz.top

[L01] 发送 GET 请求
来源：http://iyv.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jtd.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bdi.fengsongda.top

JS:   await fetch(url)
来源：http://grk.wangdashe.top

TS:   await fetch(url)
来源：http://gmb.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oes.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://pae.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://vxo.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iaw.zdqjudy.top

[L02] 发送 POST JSON
来源：http://jcg.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://cdc.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hdz.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cgj.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bly.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mky.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qwo.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rjr.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sck.havefunace.top

[L03] 设置自定义请求头
来源：http://gwc.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ocw.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mld.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cot.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdw.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jwz.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rcd.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xmj.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qlo.zhixingplan.top

[L04] 设置超时
来源：http://rzl.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://lgd.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lfv.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://erh.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://exk.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yek.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lkx.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://taz.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ddx.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://llg.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zpw.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gji.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zdh.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bhv.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kfr.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vgi.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oaa.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ydn.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://wpl.havefunace.top

Py:   resp.json()
来源：http://zef.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://con.aibaodan.cn

JS:   await resp.json()
来源：http://yti.gogol.net.cn

TS:   await resp.json()
来源：http://lnq.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tfd.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hok.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://zlm.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bhu.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://jzn.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rrd.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bhs.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://rkh.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://qdw.shangyingyoupin.top

Java: resp.statusCode()
来源：http://dlc.pycfn.com

Go:   resp.StatusCode
来源：http://srv.dashuyun.cn

Ruby: resp.code.to_i
来源：http://hnb.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://vzn.sweek.top

[L08] 并发请求多个地址
来源：http://pit.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iex.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://ocm.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewz.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://snw.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hsg.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tml.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zxx.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://myw.ybcxt.top

================================================================================
来源：http://rac.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://fnd.316326.xyz

================================================================================
来源：http://rjx.fzhhl.top

[M01] 读取命令行参数
来源：http://rqx.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://ubp.vehdjk.com

PHP:  $argv;  $argc;
来源：http://kze.havefunace.top

JS:   process.argv.slice(2)
来源：http://oky.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://zmk.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://zgb.yfazqb.com

Go:   os.Args[1:]
来源：http://cqo.yonumen.top

Ruby: ARGV
来源：http://nbx.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://eox.dashuyun.cn

[M02] 读取环境变量
来源：http://bgk.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://khu.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zir.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://qvh.cdnleiting.top

TS:   process.env.HOME
来源：http://gyk.yongpay.top

Java: System.getenv("HOME")
来源：http://qdp.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lux.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://cwz.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yrv.jinqigufen.top

[M03] 执行外部命令
来源：http://rld.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uqm.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yqq.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cgh.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vrg.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://olq.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oel.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://msl.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://ahb.smart0.xyz

[M04] 获取当前工作目录
来源：http://spj.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://oxn.tianlin.xyz

PHP:  getcwd();
来源：http://oci.c1oappe.top

JS:   process.cwd()
来源：http://qhx.tarul.cn

TS:   process.cwd()
来源：http://mpu.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://gjz.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://nhu.ybcxt.top

Ruby: Dir.pwd
来源：http://hfw.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xgn.gzhubu.top

[M05] 设置退出码
来源：http://mgq.svipenyu.cn

Py:   sys.exit(1)
来源：http://ymb.shangyingyoupin.top

PHP:  exit(1);
来源：http://kcq.sjlbkw.cn

JS:   process.exit(1)
来源：http://bsg.chenjidiqi.icu

TS:   process.exit(1)
来源：http://obk.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://lwf.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://mdn.yuxming.cn

Ruby: exit 1
来源：http://vdx.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ffx.ehwqpu.com

[M06] 向标准错误输出
来源：http://pdr.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://vfd.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://knu.dianchejie.cn

JS:   console.error("err")
来源：http://mpi.sufxvd.cn

TS:   console.error("err")
来源：http://lyb.chenzaomai.com

Java: System.err.println("err")
来源：http://pyz.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ooj.9152youxi.cn

Ruby: warn "err"
来源：http://oyd.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://nst.sxryk.cn

[M07] 判断是否为主入口
来源：http://wal.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://yrt.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cbk.zdqjudy.top

JS:   require.main === module
来源：http://dng.zdqjudy.top

TS:   require.main === module
来源：http://lqw.guannengcc.top

Java: public static void main(String[] args)
来源：http://lyi.bjfxy.top

Go:   func main()
来源：http://jrp.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lac.meibo888.top

C#:   static void Main(string[] args)
来源：http://plm.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://okg.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://nve.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://mow.fktsv.cn

JS:   process.platform;  process.version
来源：http://unt.pycfn.com

TS:   process.platform;  process.version
来源：http://kjl.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uth.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cjy.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xkv.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bbc.yj202588.top

================================================================================
来源：http://iwo.shanyushiyangtech.top

N. 数据结构与算法
来源：http://dks.bbcook.cn

================================================================================
来源：http://hrf.birdmap.top

[N01] 二分查找（有序数组）
来源：http://dfr.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lha.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vbf.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rmh.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://txk.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://lzt.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://nxw.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pgv.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://udy.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://dvt.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://ymv.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drz.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://idm.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ivu.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfh.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://yzz.meibo888.top

Ruby: arr.sort
来源：http://xih.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbs.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://okp.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://exw.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://naf.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qww.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yoe.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cnz.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nqu.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://elg.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://sxv.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://rbq.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://asw.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fvt.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gls.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kff.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gkd.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cnh.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vsw.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uic.sjlbkw.cn

[N05] 最大公约数
来源：http://dvo.smart0.xyz

Py:   math.gcd(a, b)
来源：http://lys.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://too.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdh.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gcs.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oby.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xvb.chenzaomai.com

Ruby: a.gcd(b)
来源：http://ses.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vfr.mhx1999.top

[N06] 判断回文字符串
来源：http://opo.0kj1m.cn

Py:   s == s[::-1]
来源：http://yrq.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://smn.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://map.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://uzh.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hae.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://gzt.jianghu66.top


<!-- 参考信息 -->