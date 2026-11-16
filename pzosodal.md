代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xec.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vsg.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rmq.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aav.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lpk.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iqb.feifeiyinyue.top

[J09] 时区处理
来源：http://tfw.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wxc.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wqz.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cor.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kar.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://avr.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://esr.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qgj.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vcz.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://ymx.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yoi.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://isl.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wpb.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jtu.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ofq.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aks.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gfx.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vue.fktsv.cn

================================================================================
来源：http://ojc.sjlbkw.cn

K. JSON 与序列化
来源：http://wkh.chenzaomai.com

================================================================================
来源：http://yst.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://yze.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ejc.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tjg.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://dpx.yj20258.top

TS:   JSON.stringify(obj)
来源：http://ywn.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://otl.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://loo.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dtp.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ozs.xinyue.icu

[K02] JSON 字符串转对象
来源：http://oju.nwbrower.top

Py:   json.loads(s)
来源：http://sud.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nga.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://zzu.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://xln.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hxf.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://yrq.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://lxl.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mui.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://kxg.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tbn.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gbv.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gdy.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lgz.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ayy.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rej.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://blw.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lsj.andypj.xyz

[K04] 读取 JSON 文件
来源：http://jzn.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mdu.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://krv.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqm.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://day.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://avk.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rbi.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hmw.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mya.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://evj.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://mdf.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://twk.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://tcz.jinqigufen.top

TS:   structuredClone(obj)
来源：http://idf.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cpn.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ifq.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qrm.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mbg.smart0.xyz

[K06] 解析 URL 查询串
来源：http://ica.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjq.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vef.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgy.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://prt.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://den.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ved.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://leb.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rbt.nwbrower.top

[K07] 进制转换
来源：http://mqr.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubb.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zsc.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jir.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqg.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vhj.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hab.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pht.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blh.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://mgq.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://ygh.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://luc.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://exl.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://umm.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tbn.smart0.xyz

Go:   encoding/gob
来源：http://pnr.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://fkq.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yky.fktsv.cn

================================================================================
来源：http://kzl.gzhubu.top

L. 网络请求
来源：http://kag.guowangkeji.top

================================================================================
来源：http://qpr.shzxlz.cn

[L01] 发送 GET 请求
来源：http://mmd.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rfi.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xwy.yfazqb.com

JS:   await fetch(url)
来源：http://nwe.yangfankeji.com

TS:   await fetch(url)
来源：http://wap.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ppz.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://qhy.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pjb.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://osg.yj20258.top

[L02] 发送 POST JSON
来源：http://ung.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://pgk.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lfx.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqm.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qck.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://apk.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pkw.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vgt.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwj.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://nsn.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://evn.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kym.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdv.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlo.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xkp.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ego.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ktw.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cih.fengsongda.top

[L04] 设置超时
来源：http://tmt.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://uzx.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kfd.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uda.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxf.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uyz.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygc.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vhm.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://crs.yj20258888.top

[L05] 上传文件（multipart）
来源：http://nfd.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vqn.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ucv.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fhd.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gcj.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uts.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jmh.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jiz.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://spp.gzhubu.top

[L06] 解析响应为 JSON
来源：http://frr.zhiwuduotai.top

Py:   resp.json()
来源：http://smv.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://adz.yuanzhike.top

JS:   await resp.json()
来源：http://tjk.hywenlv.cn

TS:   await resp.json()
来源：http://ifl.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xan.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gnj.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://jfd.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cvm.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://vff.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eka.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://taj.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://zxm.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://qfq.jqgfzy.top

Java: resp.statusCode()
来源：http://dqj.vqdsnc.cn

Go:   resp.StatusCode
来源：http://ato.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://tgs.meibo888.top

C#:   (int)resp.StatusCode
来源：http://ciw.yongpay.top

[L08] 并发请求多个地址
来源：http://gjx.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tii.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://dzj.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bih.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqf.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lva.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ani.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hlc.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wce.hcnkem.com

================================================================================
来源：http://xnj.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://nxt.jianghu66.top

================================================================================
来源：http://jll.yuxming.cn

[M01] 读取命令行参数
来源：http://nym.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://xvb.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://tkg.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://fvh.sweek.top

TS:   process.argv.slice(2)
来源：http://hhk.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://hrd.hnqzz.top

Go:   os.Args[1:]
来源：http://ywn.chenlongwang.top

Ruby: ARGV
来源：http://dqi.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://uut.sysykeji.top

[M02] 读取环境变量
来源：http://aop.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://dcp.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jmk.jiagoushi.top

JS:   process.env.HOME
来源：http://fjv.xziqi.cn

TS:   process.env.HOME
来源：http://hfo.fengsongda.top

Java: System.getenv("HOME")
来源：http://bun.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzw.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://tak.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ylh.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://vav.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kbj.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zso.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://prj.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tev.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hwn.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iyw.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://yvw.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://hpb.fehbvm.com

[M04] 获取当前工作目录
来源：http://svb.yuxming.cn

Py:   os.getcwd()
来源：http://pqo.zhixingplan.top

PHP:  getcwd();
来源：http://qnw.yuanzhike.top

JS:   process.cwd()
来源：http://ddu.daxiang520.top

TS:   process.cwd()
来源：http://xbu.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ksp.zycfv.cn

Go:   os.Getwd()
来源：http://ugx.hcnkem.com

Ruby: Dir.pwd
来源：http://zvw.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://fjd.jianghu66.top

[M05] 设置退出码
来源：http://bck.316326.xyz

Py:   sys.exit(1)
来源：http://wzm.meibo888.top

PHP:  exit(1);
来源：http://hqr.jqgufenzy.top

JS:   process.exit(1)
来源：http://evu.hammf.cn

TS:   process.exit(1)
来源：http://tbe.zhiwuduotai.top

Java: System.exit(1)
来源：http://ebs.c1oappe.top

Go:   os.Exit(1)
来源：http://uha.chenzaomai.com

Ruby: exit 1
来源：http://qfz.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lsg.zycfv.cn

[M06] 向标准错误输出
来源：http://uzo.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://rjw.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mui.daxiang520.top

JS:   console.error("err")
来源：http://myr.zhongyouzk.top

TS:   console.error("err")
来源：http://rxr.tian-w.cn

Java: System.err.println("err")
来源：http://lqj.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://abw.fehbvm.com

Ruby: warn "err"
来源：http://nea.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://wor.nanxinkj.top

[M07] 判断是否为主入口
来源：http://suc.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://ins.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qku.dashuyun.cn

JS:   require.main === module
来源：http://tzs.hnxiangtu.top

TS:   require.main === module
来源：http://acw.snrcjt.cn

Java: public static void main(String[] args)
来源：http://ims.wangshuangyany.cn

Go:   func main()
来源：http://psa.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://olv.52xcode.cn

C#:   static void Main(string[] args)
来源：http://ctx.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://cja.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://abr.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://hfc.yvedp.cn

JS:   process.platform;  process.version
来源：http://koq.cqqwz.cn

TS:   process.platform;  process.version
来源：http://rhq.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xbf.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zad.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mcu.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://kmb.cashguo.top

================================================================================
来源：http://ijx.sufxvd.cn

N. 数据结构与算法
来源：http://mzb.meibo888.top

================================================================================
来源：http://agc.ivvv.top

[N01] 二分查找（有序数组）
来源：http://vrt.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vuz.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eqy.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yfq.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bhd.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://tfp.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://xdp.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dar.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://uyi.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://oys.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://nnw.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://coa.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dzm.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pru.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rux.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://old.zycfv.cn

Ruby: arr.sort
来源：http://qkd.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ykv.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://jis.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cxr.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://zhw.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dmf.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lia.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbk.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://amk.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://inq.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://blk.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://enx.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vdu.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://omg.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mda.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qgx.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://imj.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hom.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://efp.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wcf.hnqzz.top

[N05] 最大公约数
来源：http://trv.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://wrc.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://man.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iiu.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nbg.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pdf.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brs.sysykeji.top

Ruby: a.gcd(b)
来源：http://opq.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tjt.nwbrower.top

[N06] 判断回文字符串
来源：http://uyv.havefunace.top

Py:   s == s[::-1]
来源：http://muc.xinyue.icu

PHP:  $s === strrev($s);
来源：http://ukp.yongpay.top


<!-- 参考信息 -->