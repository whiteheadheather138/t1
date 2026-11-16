代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iii.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kxy.yuxming.cn

[J09] 时区处理
来源：http://cuq.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xyi.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oqs.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://puc.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckg.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vkw.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gal.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hmq.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bht.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://cps.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://njt.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jmg.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qrm.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tyn.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsd.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iwm.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aji.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vyn.chenjidiqi.icu

================================================================================
来源：http://vgc.meibo888.top

K. JSON 与序列化
来源：http://erg.haohaochexian.top

================================================================================
来源：http://zfd.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://cip.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oaw.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vpz.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://kog.cheryme.top

TS:   JSON.stringify(obj)
来源：http://sjq.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldp.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://snx.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ndg.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nea.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://fae.sufxvd.cn

Py:   json.loads(s)
来源：http://xlk.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sea.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://ods.jqgfzy.top

TS:   JSON.parse(s)
来源：http://btt.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fep.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://gba.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://tqv.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gml.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://wgs.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nnl.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bdq.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hsb.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hba.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uko.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pwl.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://auj.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zmd.fzhhl.top

[K04] 读取 JSON 文件
来源：http://iwd.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iwb.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xzn.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emg.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://keu.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ubw.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lvp.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wlu.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hph.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://fei.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://vhc.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://afo.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://zqk.zycfv.cn

TS:   structuredClone(obj)
来源：http://yse.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://efb.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ooy.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pze.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vbv.birdmap.top

[K06] 解析 URL 查询串
来源：http://gyd.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hda.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ars.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyv.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfg.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubg.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://klh.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fmm.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tln.zhoulong.xyz

[K07] 进制转换
来源：http://pez.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dze.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jnq.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nav.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vob.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vgt.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://itt.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sab.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pkw.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://qou.havefunace.top

Py:   pickle.dumps(obj)
来源：http://ley.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://eis.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://bbu.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://lab.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hqa.hongshengwenyu.top

Go:   encoding/gob
来源：http://ibb.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://dcd.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://epv.hywenlv.cn

================================================================================
来源：http://rwr.guowangkeji.top

L. 网络请求
来源：http://zod.jlsjyb.cn

================================================================================
来源：http://uan.snrcjt.cn

[L01] 发送 GET 请求
来源：http://wga.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rwh.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vji.shzxlz.cn

JS:   await fetch(url)
来源：http://nfw.ctjpmb.com

TS:   await fetch(url)
来源：http://zgv.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mlx.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://dmq.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eyq.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rmm.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://nnq.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://nlq.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://twk.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://npb.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbe.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qiz.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qnx.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yxx.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rvj.xziqi.cn

[L03] 设置自定义请求头
来源：http://dhd.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://daw.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uha.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rmc.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://non.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gmy.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qiw.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dnr.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yrv.vqdsnc.cn

[L04] 设置超时
来源：http://ypf.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://jad.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dsr.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gri.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cog.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aqr.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bbi.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ste.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hsu.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://uiv.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gck.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hwk.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqq.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kqu.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xpf.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tpb.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjn.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qjj.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://aar.cheryme.top

Py:   resp.json()
来源：http://her.yj20258.top

PHP:  json_decode($body, true);
来源：http://tje.gzhubu.top

JS:   await resp.json()
来源：http://wya.quarkkingdee.top

TS:   await resp.json()
来源：http://qbx.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qyu.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://toc.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://wyl.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://efe.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://gom.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xym.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://smw.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://piv.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://gza.jqgfzy.top

Java: resp.statusCode()
来源：http://oet.yonumen.top

Go:   resp.StatusCode
来源：http://ded.fktsv.cn

Ruby: resp.code.to_i
来源：http://ezh.pycfn.com

C#:   (int)resp.StatusCode
来源：http://eod.svipenyu.cn

[L08] 并发请求多个地址
来源：http://kdd.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vhm.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://zux.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwq.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yav.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://beh.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cqu.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xsu.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lme.sysykeji.top

================================================================================
来源：http://dcq.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://ahk.ydzc1.top

================================================================================
来源：http://aky.guowangkeji.top

[M01] 读取命令行参数
来源：http://xxq.sweek.top

Py:   sys.argv[1:]
来源：http://qfc.shuidangran.top

PHP:  $argv;  $argc;
来源：http://tgv.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://vyi.sweek.top

TS:   process.argv.slice(2)
来源：http://lqg.yj202588.top

Java: args 数组（main 方法参数）
来源：http://mfm.yj20258.top

Go:   os.Args[1:]
来源：http://gmd.vehdjk.com

Ruby: ARGV
来源：http://tkp.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://idm.hywenlv.cn

[M02] 读取环境变量
来源：http://egx.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://ukj.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cjx.hammf.cn

JS:   process.env.HOME
来源：http://gnj.ybcxt.top

TS:   process.env.HOME
来源：http://iae.hfpthk.cn

Java: System.getenv("HOME")
来源：http://mop.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://utg.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://iau.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://isi.yuxming.cn

[M03] 执行外部命令
来源：http://bbe.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://flb.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://slu.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nhh.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nlr.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://evy.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://awc.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://vom.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://qzb.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://bel.52xcode.cn

Py:   os.getcwd()
来源：http://uuf.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://wgz.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://njb.mhx1999.top

TS:   process.cwd()
来源：http://axv.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://fae.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://dli.52xcode.cn

Ruby: Dir.pwd
来源：http://kqz.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://mlo.zhoulong.xyz

[M05] 设置退出码
来源：http://mdj.daria6918.cn

Py:   sys.exit(1)
来源：http://gdv.quarkkingdee.top

PHP:  exit(1);
来源：http://nqe.ydzc1.top

JS:   process.exit(1)
来源：http://vpi.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://yhy.sjlbkw.cn

Java: System.exit(1)
来源：http://jia.ydjk.org.cn

Go:   os.Exit(1)
来源：http://pdr.meibo888.top

Ruby: exit 1
来源：http://qnw.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ngw.cheryme.top

[M06] 向标准错误输出
来源：http://ajy.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://wbr.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vfb.yuxming.cn

JS:   console.error("err")
来源：http://tqr.yuanzhike.top

TS:   console.error("err")
来源：http://fyc.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ady.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hlf.xylfe.cn

Ruby: warn "err"
来源：http://inc.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://jwh.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://tel.tanke756.top

Py:   if __name__ == "__main__":
来源：http://srr.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vcu.uphjek.com

JS:   require.main === module
来源：http://wst.tianlin.xyz

TS:   require.main === module
来源：http://eit.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://gjq.shuidangran.top

Go:   func main()
来源：http://zki.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vuu.daxiang520.top

C#:   static void Main(string[] args)
来源：http://knu.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://krl.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://wqn.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://xxc.aizwys.cn

JS:   process.platform;  process.version
来源：http://ohv.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://yau.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mlh.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://amp.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lih.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eym.uphjek.com

================================================================================
来源：http://pnk.epnwcf.com

N. 数据结构与算法
来源：http://gug.yuxming.cn

================================================================================
来源：http://aui.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://daf.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://wzi.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vwz.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uug.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cov.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://xsp.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://tib.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dtp.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://zgw.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://vpc.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://gsf.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gma.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://adm.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bax.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wxr.pycfn.com

Go:   slices.Sort(arr)
来源：http://zjz.yongpay.top

Ruby: arr.sort
来源：http://eio.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://iuq.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://uok.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gca.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://nql.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eih.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hvf.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wut.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://anz.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfl.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wtu.ydzc1.top

[N04] 斐波那契数列
来源：http://eqq.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kre.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cxt.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://org.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewm.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pei.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qio.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kxj.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hzt.hongshengwenyu.top

[N05] 最大公约数
来源：http://qzu.ybcxt.top

Py:   math.gcd(a, b)
来源：http://gin.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mop.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyt.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hlw.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uzw.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ynu.zdbjq.cn

Ruby: a.gcd(b)
来源：http://awg.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ctd.xuanzx.com

[N06] 判断回文字符串
来源：http://yzv.meibo888.top

Py:   s == s[::-1]
来源：http://tzl.havefunace.top

PHP:  $s === strrev($s);
来源：http://fye.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://ofb.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://ujo.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vvv.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://flf.sysykeji.top


<!-- 参考信息 -->