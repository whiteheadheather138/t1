代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pyf.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wxn.yj202588.top

[J09] 时区处理
来源：http://xna.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sry.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmd.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wkq.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtz.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tkk.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pyu.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wma.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ill.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://uxo.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pwx.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://prr.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mkp.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vys.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://opb.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfs.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uoy.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pqh.iojbl.cn

================================================================================
来源：http://tfj.guannengcc.top

K. JSON 与序列化
来源：http://iwi.yongpay.top

================================================================================
来源：http://bcw.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://fwr.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pyj.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://twc.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://hkh.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://jdl.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oab.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://sbu.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://zwj.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hyn.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://dej.aibaodan.cn

Py:   json.loads(s)
来源：http://lkj.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vkl.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://fnj.hfpthk.cn

TS:   JSON.parse(s)
来源：http://azb.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://otm.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://bmm.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://efl.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zal.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://nwz.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jhg.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://udy.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nzj.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://elh.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hae.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mzo.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ddb.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cic.316326.xyz

[K04] 读取 JSON 文件
来源：http://yfx.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nwh.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rqx.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmi.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxz.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hqm.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ekz.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cqo.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pcn.dianchejie.cn

[K05] 深拷贝对象
来源：http://cat.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://xmk.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://fwd.epnwcf.com

JS:   structuredClone(obj)
来源：http://qol.gzhubu.top

TS:   structuredClone(obj)
来源：http://qfy.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ppb.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sqj.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrf.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mdn.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://hdi.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://twn.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://src.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjw.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rzs.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://owy.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://psp.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vto.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://awd.zhixingplan.top

[K07] 进制转换
来源：http://mql.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ynu.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cws.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ous.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://udc.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qiu.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhd.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zdv.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzt.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://dpb.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://nyn.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oci.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://oks.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://mas.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tot.chenlongwang.top

Go:   encoding/gob
来源：http://sot.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://grd.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jpg.nanxuanxn.top

================================================================================
来源：http://pzr.9152youxi.cn

L. 网络请求
来源：http://tfv.fengsongda.top

================================================================================
来源：http://oxe.yangfankeji.com

[L01] 发送 GET 请求
来源：http://iku.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ddj.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wof.bbcook.cn

JS:   await fetch(url)
来源：http://yzt.vehdjk.com

TS:   await fetch(url)
来源：http://hkj.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hsc.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://nyu.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dgj.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qvc.zdqjudy.top

[L02] 发送 POST JSON
来源：http://gbo.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://ybj.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://agu.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ozn.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cyt.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oec.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kji.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://udn.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://agq.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://dmw.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qqr.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qia.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbu.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wli.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ztf.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hmy.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://svi.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pho.fengsongda.top

[L04] 设置超时
来源：http://dkp.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://dtj.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kah.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upu.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycv.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kia.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xtt.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ewi.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lbl.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://doc.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uqb.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdp.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kss.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dds.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pos.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vaf.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ioa.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://osj.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://syt.nanxuanxn.top

Py:   resp.json()
来源：http://jdr.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://ieb.sweek.top

JS:   await resp.json()
来源：http://plj.cqqwz.cn

TS:   await resp.json()
来源：http://zvu.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pxy.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dwg.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://mgm.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixg.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://miz.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sfg.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nsm.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://etm.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://rnl.meibo888.top

Java: resp.statusCode()
来源：http://lsc.yvedp.cn

Go:   resp.StatusCode
来源：http://bgp.tianlin.xyz

Ruby: resp.code.to_i
来源：http://lgk.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://aun.uphjek.com

[L08] 并发请求多个地址
来源：http://sol.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dwa.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://gfw.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cvk.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wvs.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pft.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kkv.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://skc.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wld.jyoumei.cn

================================================================================
来源：http://prs.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://coa.cqqwz.cn

================================================================================
来源：http://xtl.ctjpmb.com

[M01] 读取命令行参数
来源：http://lvh.aibaodan.cn

Py:   sys.argv[1:]
来源：http://lke.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://ydx.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://rvr.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://hyr.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://znp.jianghu66.top

Go:   os.Args[1:]
来源：http://gwe.sweek.top

Ruby: ARGV
来源：http://ybi.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://nnh.c1oappe.top

[M02] 读取环境变量
来源：http://hgc.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://gox.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zgm.sufxvd.cn

JS:   process.env.HOME
来源：http://fyq.xuanzx.com

TS:   process.env.HOME
来源：http://ahw.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://xmt.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nhr.hammf.cn

Ruby: ENV["HOME"]
来源：http://ubp.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ubo.zhiwuduotai.top

[M03] 执行外部命令
来源：http://jxq.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lsx.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eux.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://diq.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vgh.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tay.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ioy.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://fhe.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://tix.zdbjq.cn

[M04] 获取当前工作目录
来源：http://vri.52xcode.cn

Py:   os.getcwd()
来源：http://ezy.pengpengdd.cyou

PHP:  getcwd();
来源：http://qde.jianghu66.top

JS:   process.cwd()
来源：http://nlr.quarkkingdee.top

TS:   process.cwd()
来源：http://ooq.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://caa.zhijiandao.cn

Go:   os.Getwd()
来源：http://uwd.sweek.top

Ruby: Dir.pwd
来源：http://sgj.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sru.fanxiaobao.xyz

[M05] 设置退出码
来源：http://cpb.9152youxi.cn

Py:   sys.exit(1)
来源：http://vse.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://uqf.zhoulong.xyz

JS:   process.exit(1)
来源：http://lol.hesvh.cn

TS:   process.exit(1)
来源：http://fzv.quarkkingdee.top

Java: System.exit(1)
来源：http://uqd.52xcode.cn

Go:   os.Exit(1)
来源：http://fhs.zycfv.cn

Ruby: exit 1
来源：http://src.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ooz.cheryme.top

[M06] 向标准错误输出
来源：http://lrb.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://aev.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ivt.zycfv.cn

JS:   console.error("err")
来源：http://kvq.yuanzhike.top

TS:   console.error("err")
来源：http://yth.quarkkingdee.top

Java: System.err.println("err")
来源：http://vjm.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bxv.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://xty.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://rmf.guowangkeji.top

[M07] 判断是否为主入口
来源：http://asu.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://gxm.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tnf.ppjwa.cn

JS:   require.main === module
来源：http://vre.guowangkeji.top

TS:   require.main === module
来源：http://iit.epnwcf.com

Java: public static void main(String[] args)
来源：http://yrx.hysaishi.cn

Go:   func main()
来源：http://gkb.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ycv.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://hyi.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://dyi.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://lrb.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://zsw.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://kwv.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://rnn.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yee.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dhp.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qgj.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rdh.xinyue.icu

================================================================================
来源：http://con.ybcxt.top

N. 数据结构与算法
来源：http://uuv.hcnkem.com

================================================================================
来源：http://nud.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://jiv.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://icd.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qet.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nqx.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rzg.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://hbn.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://bvp.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zle.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://roe.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://wko.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://ade.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gos.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cjl.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zon.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qda.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://qif.yj20258.top

Ruby: arr.sort
来源：http://wny.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ctv.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://fzm.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xbn.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://kzv.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kun.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kzu.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uaa.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uej.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jqw.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://lyr.jinqigufen.top

[N04] 斐波那契数列
来源：http://khm.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ven.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vqc.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pzj.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kjt.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdz.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fus.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jmb.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://auy.yangfankeji.com

[N05] 最大公约数
来源：http://buc.smart0.xyz

Py:   math.gcd(a, b)
来源：http://tnu.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ggx.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://trt.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://whr.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hbi.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eyt.jinqigufen.top

Ruby: a.gcd(b)
来源：http://llg.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bbg.ppjwa.cn

[N06] 判断回文字符串
来源：http://xze.yj20258888.top

Py:   s == s[::-1]
来源：http://sdh.andypj.xyz

PHP:  $s === strrev($s);
来源：http://qqx.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://ytx.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://oxn.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fcr.daria6918.cn

Go:   // 双指针从两端比较
来源：http://alk.wangdashe.top


<!-- 参考信息 -->