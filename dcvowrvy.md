代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://svr.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obc.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://elc.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://coy.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kik.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://klv.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fui.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://oao.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://szm.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://joq.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://udq.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oon.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xay.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yrl.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://isv.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pof.hnqzz.top

================================================================================
来源：http://pyo.ppjwa.cn

K. JSON 与序列化
来源：http://yyg.tian-w.cn

================================================================================
来源：http://zcg.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://cgd.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvr.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bdq.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://rfd.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://crl.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hsd.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://vgt.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dtg.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://wnm.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://enp.zdqjudy.top

Py:   json.loads(s)
来源：http://lbo.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qew.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://jyn.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://spe.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yon.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://jut.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://jza.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vte.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://ynq.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://stx.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ide.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pkk.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jzn.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://itp.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wcn.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ukx.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://phy.hnqzz.top

[K04] 读取 JSON 文件
来源：http://cbo.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zvu.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icw.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afw.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gzx.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://opr.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vik.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzs.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dya.zdqjudy.top

[K05] 深拷贝对象
来源：http://oer.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://nyh.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://dan.cdnleiting.top

JS:   structuredClone(obj)
来源：http://imi.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://nux.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gck.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jnz.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jlm.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tsw.hesvh.cn

[K06] 解析 URL 查询串
来源：http://qvw.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wzo.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jbg.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jeb.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfd.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bnx.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ffr.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jnl.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fwx.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://qey.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://avb.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fnb.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sze.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kax.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ohk.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rgy.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://att.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dwd.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://sor.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://xxk.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fos.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://krj.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://ofb.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xym.epnwcf.com

Go:   encoding/gob
来源：http://vel.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://qyj.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://raj.sufxvd.cn

================================================================================
来源：http://bzv.jinyuanbaomall.cn

L. 网络请求
来源：http://stn.yfazqb.com

================================================================================
来源：http://pbq.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://tkc.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qun.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iir.ydzc1.top

JS:   await fetch(url)
来源：http://ope.mhx1999.top

TS:   await fetch(url)
来源：http://wwf.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fex.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://pwe.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gjc.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nyp.hfpthk.cn

[L02] 发送 POST JSON
来源：http://rjk.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://zuz.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rzz.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfe.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://voh.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lys.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blc.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cxt.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://soq.fktsv.cn

[L03] 设置自定义请求头
来源：http://hww.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zgo.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://abc.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sco.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bby.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzl.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sum.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pqj.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vvu.hnxiangtu.top

[L04] 设置超时
来源：http://uls.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://mky.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehx.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hnb.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lwi.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cpv.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lrd.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iht.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://unm.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://min.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dmi.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tay.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyz.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pqd.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lmw.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aze.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrx.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dug.yj20258888.top

[L06] 解析响应为 JSON
来源：http://bmv.ehwqpu.com

Py:   resp.json()
来源：http://fdf.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://jfz.52xcode.cn

JS:   await resp.json()
来源：http://cgb.dianchejie.cn

TS:   await resp.json()
来源：http://emo.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gfb.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bfe.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://uem.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://owk.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://kqu.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcy.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upf.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://lop.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://rmw.hnxiangtu.top

Java: resp.statusCode()
来源：http://ejx.vqdsnc.cn

Go:   resp.StatusCode
来源：http://bzw.sxryk.cn

Ruby: resp.code.to_i
来源：http://rmq.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://fgl.52xcode.cn

[L08] 并发请求多个地址
来源：http://emt.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xlv.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://rko.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ljz.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rqk.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xom.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://keq.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ver.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ett.zhaomingkeji.xyz

================================================================================
来源：http://qlx.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://mir.jqgfzy.top

================================================================================
来源：http://snn.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://adj.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://ema.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://znt.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://gii.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://mof.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://oyr.jlsjyb.cn

Go:   os.Args[1:]
来源：http://bkh.yongpay.top

Ruby: ARGV
来源：http://ryz.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://hlf.hammf.cn

[M02] 读取环境变量
来源：http://wyy.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://qog.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqy.pycfn.com

JS:   process.env.HOME
来源：http://pqs.jinqigufen.top

TS:   process.env.HOME
来源：http://mpt.yvedp.cn

Java: System.getenv("HOME")
来源：http://cgv.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oaf.hammf.cn

Ruby: ENV["HOME"]
来源：http://bvr.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aqt.jyoumei.cn

[M03] 执行外部命令
来源：http://fbd.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://glg.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://osi.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lej.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://rib.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kei.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://njy.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://nni.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://hsm.yonumen.top

[M04] 获取当前工作目录
来源：http://lma.hammf.cn

Py:   os.getcwd()
来源：http://bfs.nwbrower.top

PHP:  getcwd();
来源：http://wkb.zdbjq.cn

JS:   process.cwd()
来源：http://jns.jqgfzy.top

TS:   process.cwd()
来源：http://xap.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://zzb.gzhubu.top

Go:   os.Getwd()
来源：http://qyj.yonumen.top

Ruby: Dir.pwd
来源：http://rce.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://apz.yangfankeji.com

[M05] 设置退出码
来源：http://xcr.aibaodan.cn

Py:   sys.exit(1)
来源：http://bzd.chenjidiqi.icu

PHP:  exit(1);
来源：http://yle.xinyue.icu

JS:   process.exit(1)
来源：http://agl.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://xvf.chenjidiqi.icu

Java: System.exit(1)
来源：http://kzj.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://swo.xinyue.icu

Ruby: exit 1
来源：http://xpg.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ddu.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://ttk.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://gqe.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fqf.xylfe.cn

JS:   console.error("err")
来源：http://fac.aizwys.cn

TS:   console.error("err")
来源：http://ift.jqgfzy.top

Java: System.err.println("err")
来源：http://pmm.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ruv.fktsv.cn

Ruby: warn "err"
来源：http://vev.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://mvb.xinyue.icu

[M07] 判断是否为主入口
来源：http://msf.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://edx.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dzd.shanyushiyangtech.top

JS:   require.main === module
来源：http://mef.tianlin.xyz

TS:   require.main === module
来源：http://kmu.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://nrf.zdbjq.cn

Go:   func main()
来源：http://xhw.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://evb.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://wpd.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://zse.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://lmm.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://npg.daria6918.cn

JS:   process.platform;  process.version
来源：http://owg.yangfankeji.com

TS:   process.platform;  process.version
来源：http://evx.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mzn.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xby.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ata.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://avb.xylfe.cn

================================================================================
来源：http://abw.ctjpmb.com

N. 数据结构与算法
来源：http://xcs.nanxinkj.top

================================================================================
来源：http://qni.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://yay.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://heo.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rmq.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://umc.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkb.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wao.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://nxc.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://fci.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://zrv.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://dll.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://vth.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jtc.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jsn.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://heb.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ehe.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://cea.sufxvd.cn

Ruby: arr.sort
来源：http://tsr.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbo.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://hew.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nih.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://qrd.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfo.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mre.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bqo.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://llq.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dhm.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://ckl.jyoumei.cn

[N04] 斐波那契数列
来源：http://aae.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yxy.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipp.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uch.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://edv.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uxb.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxw.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hkl.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rjs.xuanzx.com

[N05] 最大公约数
来源：http://tvv.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://ezh.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://omk.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dsi.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oke.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jpa.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dls.guannengcc.top

Ruby: a.gcd(b)
来源：http://ngu.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwt.zhengqikj.top

[N06] 判断回文字符串
来源：http://tok.yuanzhike.top

Py:   s == s[::-1]
来源：http://cwp.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://nra.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://xtj.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://okc.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fhv.xuanzx.com

Go:   // 双指针从两端比较
来源：http://rxp.andypj.xyz

Ruby: s == s.reverse
来源：http://vdp.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ihb.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://sru.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://npk.shuidangran.top


<!-- 参考信息 -->